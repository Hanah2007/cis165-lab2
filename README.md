# CIS-165 Lab 2

## Program Plans

### Program 1 — Sum of Two Numbers

I will store 50 and 100 in integer variables. I will add the two variables together and store the result in a variable named total. Then I will display total with a clear label.

### Program 2 — Miles Per Gallon

I will store 312 miles and 16 gallons in variables. I will divide the miles by the gallons to calculate miles per gallon and store the result in a variable. I will use a data type that preserves the fractional result and display the result with the MPG unit.



\## Testing



| Program/Test                | Values Used           | Expected Result | Actual Output                 | Match or Correction |

| --------------------------- | --------------------- | --------------- | ----------------------------- | ------------------- |

| `sum.cpp` — assigned values | 50 and 100            | Total = 150     | Total: 150                    | Match               |

| `sum.cpp` — changed values  | 25 and 75             | Total = 100     | Total: 100                    | Match               |

| `mpg.cpp` — assigned values | 312 miles; 16 gallons | 19.5 MPG        | Miles per gallon: 19.5 MPG    | Match               |

| `mpg.cpp` — changed values  | 250 miles; 12 gallons | 20.8333... MPG  | Miles per gallon: 20.8333 MPG | Match               |



The temporary test values were restored before the final runs. The final versions of both programs use the original assigned values from the lab instructions.



\## Code Explanations



\### sum.cpp



The program stores 50 in `first\_number` and 100 in `second\_number`. It adds those two variables and stores the result in `total`, which gives 150. The program then displays the value stored in `total`.



The calculation is stored in `total` before printing because the assignment requires the calculation to be completed first and then the result variable to be displayed. This also makes the code easier to read and understand.



\### mpg.cpp



The program calculates miles per gallon using the formula:



`miles per gallon = miles / gallons`



For the assigned values, the calculation is 312 divided by 16, which gives 19.5 MPG. The program uses `double` for the miles, gallons, and MPG variables so that fractional results can be preserved.



If C++ performs division using two integer operands, integer division can discard the decimal portion of the result. Using `double` allows the program to keep the fractional portion.



For the changed-value test, the program used 250 miles and 12 gallons. The calculation was 250 divided by 12, which gives approximately 20.8333 MPG. The program produced `20.8333 MPG`, matching the expected fractional result.



\## How to Compile and Run



Using a C++ compiler with C++17 support:



```text

g++ -std=c++17 -Wall -Wextra sum.cpp -o sum

./sum



g++ -std=c++17 -Wall -Wextra mpg.cpp -o mpg

./mpg

```



The two programs should be compiled and run separately because each program has its own `main()` function.



The programs were written and tested using OnlineGDB.



