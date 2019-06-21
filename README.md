# arches-csv-formatting-tool
# Aims: 
1. Indentify values containing "$"  
2. Split these values and put them on a new 'blank' row in the same column
3. Give these new lines the same ResoruceID as the row they were found


# Example 
| ResourceID  | Subject(s) |
|---|---|
| 1 |  A |
| 2 | B $ C $ D|
| 3 | E $ F |

 Needs to be converted to this... 

| ResourceID  | Subject(s) |
|---|---|
| 1 | A |
| 2 | B |
| 2 | C |
| 2 | D |
| 3 | E |
| 3 | F |

# Code...
Initial ideas and working in .ipynb files
