# **Module 1: Basic Concepts**  

Rules in this module are written using the **Standard Verification Rule Format (SVRF)**.  

<br />

## Main Commands for Statement Syntax

1. **DRC Maximum Results**  
   > Defines the maximum number of results reported per DRC rule.  
   > **Syntax**: `DRC MAXIMUM RESULTS {all | value}`  
   > **Example**: `DRC MAXIMUM RESULTS all`

2. **DRC Summary Report**  
   > Defines the summary report file and the method used to write to it.  
   > **Syntax**: `DRC SUMMARY REPORT {Replace | Append}`  
   > **Example**: `DRC SUMMARY REPORT 'drc_report' Replace`


3. **DRC RESULTS DATABASE**  
   > Defines the results file name and the type of it.  
   > **Syntax**: `DRC RESULTS DATABASE {filename} {ASCII | GDS | OASIS}`  
   > **Example**: `DRC RESULTS DATABASE "drc.db" GDSII`


4. **Layout System**  
   > Defines the format of the input layout file.  
   > **Syntax**: `LAYOUT SYSTEM {GDSII | OASIS}`  
   > **Example**: `LAYOUT SYSTEM GDS`

5. **Layout Path**  
   > Defines the file path of the input layout.  
   > **Syntax**: `LAYOUT PATH {path_to_file}`  
   > **Example**: `LAYOUT PATH "/home/designs/chip.gds"`

6. **Layout Primary**  
   > Defines the name of the top-level cell in the layout.  
   > **Syntax**: `LAYOUT PRIMARY {top_cell_name}`  
   > **Example**: `LAYOUT PRIMARY "TOP"`

