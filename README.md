Solve sudoku with Constraint Propagation

**The "Naked Twins" Strategy**
The To find the naked twins we
- gather as candidates the boxes (within the units) with only two digits  
- combine them in pairs  
- find identical pairs (the ones with the same values)  
so these are the naked twins. 
Then we remove the values of the naked-twin from theier peers in the unit. 
We use the naked twins strategy in conbination with the eliminate and only choice strategies repetitevly (constraint propagation) until the puzzle stops changing. 
 
**Constraint propagation**
Constraint propagation is used to solve the diagonal sudoku problem as follows:
- Encode the Board as the regular sudoku puzzle with rows, columns and square units
- Identify and encode boxes of the two diagonal units and add them to the existing unit list
- Use the eliminate, only choice, naked twins strategies repetitivly until the puzzle stops changing (as we did while solving the regular sudoku problem)
