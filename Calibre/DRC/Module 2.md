# **Module 2: DRC Basics**  
Rules in this module are written using the **Standard Verification Rule Format (SVRF)**.  

<br />

## Main Commands in This Module

1. **LAYER**  
   > Defines the original layers to be used in rule checks.  
   > **Syntax**: `LAYER {layer_name_in_rule_file} {layer_number}`  
   > **Example**: `LAYER POLY 5`

2. **LAYOUT WINDOW**  
   > Specifies the region of the layout to be checked during rule check.  
   > **Syntax**: `LAYOUT WINDOW x1 y1 x2 y2`  
   > **Example**: `LAYOUT WINDOW 10 3 30 25`

