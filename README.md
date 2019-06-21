# arches-csv-formatting-tool
# Aims: 
1. Indentify values containing "$"  
2. Split these values and put them on a new 'blank' row in the same column
3. Give these new lines the same ResoruceID as the row they were found


# Example 
| ResourceID  | Column 1 | Column 2 | 
|---|---|---|
| 1 |  A | X | 
| 2 | B $ C $ D| Y |
| 3 | E $ F | Z |

 Needs to be converted to this... 

| ResourceID  | Column 1 | Column 2 |
|---|---|---|
| 1 | A | X | 
| 2 | B | Y | 
| 2 | C |   |
| 2 | D |   |
| 3 | E | Z |
| 3 | F |   |

# Code...
Initial ideas and working is located in .ipynb files. The above example is example_data.csv.
