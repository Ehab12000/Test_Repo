# **Module 4: Polygon-Directed Rule Checks**  

Rules in this module are written using the **Standard Verification Rule Format (SVRF)**.  

<br />

## **Boolean Operations**

1. **AND**  
 > * Selects all polygon areas that are common between specific polygons.  
 > **Syntax**: `AND {layer1} {layer2}`  
 > **Example**: `AND L1 L2`

2. **OR**  
 > * Selects the combined area of both polygons.  
 > **Syntax**: `OR {layer1} {layer2}`  
 > **Example**: `OR L1 L2`

3. **NOT**  
 > * Selects all polygon areas in layer1 that are not common to the polygon areas in layer2.  
 > **Syntax**: `NOT {layer1} {layer2}`  
 > **Example**: `NOT L1 L2`

4. **XOR**  
 > * Selects the area of the polygons excluding the common area.  
 > **Syntax**: `XOR {layer1} {layer2}`  
 > **Example**: `XOR L1 L2`

<br />

## **Topological Operations**

1. **DONUT**  
 > * Selects polygons that contain holes without selecting the holes themselves.  
 > **Syntax**: `DONUT {layer} {constraints_number_of_holes}`  
 > **Example**: `DONUT L1 <= 2`

2. **HOLES**  
 > * Selects the holes within a polygon.  
 > **Syntax**: `HOLES {layer} {constraints_area_of_holes}`  
 > **Example**: `HOLES L1 < 2`

3. **INSIDE**  
 > * Selects polygons that are completely inside layer2 polygons.  
 > **Syntax**: `INSIDE {layer1} {layer2}`  
 > **Example**: `INSIDE L1 L2`

4. **OUTSIDE**  
 > * Selects polygons in layer1 that are completely outside layer2 polygons.  
 > **Syntax**: `OUTSIDE {layer1} {layer2}`  
 > **Example**: `OUTSIDE L1 L2`

5. **TOUCH**  
 > * Selects polygons that exist outside another polygon but share an edge with it.  
 > **Syntax**: `TOUCH {layer1} {layer2}`  
 > **Example**: `TOUCH L1 L2`

6. **AREA**  
 > * Selects polygons with areas that satisfy the specified constraint.  
 > **Syntax**: `AREA {layer1} {constraint}`  
 > **Example**: `AREA L1 < 6`

7. **WITH EDGE**  
 > * Selects polygons that share an edge with another layer's polygons, without needing to be outside.  
 > **Syntax**: `{layer1} WITH EDGE {layer2}`  
 > **Example**: `L2 WITH EDGE L1`

