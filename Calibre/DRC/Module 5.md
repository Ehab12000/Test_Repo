# **Module 5: Edge and Error-Directed Checks**

Rules in this module are written using the **Standard Verification Rule Format (SVRF)**.  

<br />

## **EDGE-DIRECTED CHECKS**

1. **INSIDE EDGE**  
 > * Selects edges that lie completely inside layer2 polygons.  
 > **Syntax**: `INSIDE EDGE {layer1} {layer2}`  
 > **Example**: `INSIDE EDGE L1 L2`

2. **OUTSIDE EDGE**  
 > * Selects edges that lie completely outside layer2 polygons.  
 > **Syntax**: `OUTSIDE EDGE {layer1} {layer2}`  
 > **Example**: `OUTSIDE EDGE L1 L2`

3. **LENGTH**  
 > * Selects edges whose length satisfies the specified constraints.  
 > **Syntax**: `LENGTH {layer} {constraint}`  
 > **Example**: `LENGTH L1 < 5`

4. **PATH LENGTH**  
 > * Selects edges in a chain that satisfy the specified constraints.  
 > **Syntax**: `PATH LENGTH {layer1} {constraint}`  
 > **Example**: `PATH LENGTH L1 < 10`

5. **XOR**  
 > * Selects the area of the polygons excluding the common area.  
 > **Syntax**: `XOR {layer1} {layer2}`  
 > **Example**: `XOR L1 L2`

<br />

## **ERROR-DIRECTED CHECKS**

1. **DRAWN ACUTE**  
 > * Generates a derived error layer containing acute angles.

2. **DRAWN SKEW**  
 > * Generates a derived error layer containing skewed edges.

