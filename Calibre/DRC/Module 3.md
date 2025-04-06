# **Module 3: Dimensional Rule Checks**  

Rules in this module are written using the **Standard Verification Rule Format (SVRF)**.  

<br />

## **DRC Rule Check Operation Commands**

1. **INTERNAL**  
 > * Checks the width of a polygon.  
 > **Syntax**: `INT {layer} {constraint} {secondary keywords}`  
 > **Example**: `INT L1 < 2`  
 > * Checks the overlap width between different polygons.  
 > **Syntax**: `INT {layer1} {layer2} {constraint} {secondary keywords}`  
 > **Example**: `INT L1 L2 <= 2`

2. **EXTERNAL**  
 > * Checks the spacing between the edges of polygons.  
 > **Syntax**: `EXT {layer1} {layer2} {constraint} {secondary keywords}`  
 > **Example**: `EXT L1 < 2` — spacing between edges of the same polygon  
 > **Example**: `EXT L1 L2 < 2` — spacing between edges of different polygons

3. **ENCLOSURE**  
 > * Checks enclosures and extensions.  
 > **Syntax**: `ENC {layer1} {layer2} {constraint} {secondary keywords}`  
 > **Example**: `ENC L1 L2 < 4`

<br />

## **Secondary Keywords**  
Secondary keywords can be added to DRC operation commands to refine rule definitions.

1. **ABUT**  
 > * Measures the separation between abutting edge pairs based on angular separation, and compares it against the constraint.  
 > **Example**: `EXT L1 L2 < 1 ABUT == 90`

2. **SINGULAR**  
 > * Measures the separation between intersecting edge pairs at polygon vertices.
 > **Example**: `INT L1 L2 < 0.5 SINGULAR`

3. **PARALLEL**  
 > * Measures spacing between parallel edges.  
 > **Example**: `EXT L1 L2 < 0.5 PARALLEL`

4. **PERPENDICULAR**  
 > * Measures spacing between perpendicular edges.  
 > **Example**: `ENC L1 L2 < 0.5 PERPENDICULAR`

5. **CONNECTED**  
 > * Measures separation between polygons that belong to the same net.  
 > **Example**: `EXT L1 L2 < 1 CONNECTED`

