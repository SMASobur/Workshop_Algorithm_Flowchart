# Workshop: Algorithm and Flowchart

For each question in this workshop, you must complete **two** things:

1.  **Write the pseudocode**
2.  **Draw the flowchart** using either
    - **Option 1:** Draw.io (recommended) → export image → upload to
      your repository → link it in this file
    - **Option 2 (optional):** Write a Mermaid flowchart directly in
      Markdown
    - **Option 3 (optional):** Any other valid method

👉 **IMPORTANT:** At the **bottom of each question**, add the
following sections:

### ✔ Pseudocode

### ✔ Flowchart

---

## 1. Check Even or Odd Number

Design an algorithm and flowchart that take a number as input and
determine whether it is even or odd.

### ✔ Pseudocode

```text
START
    INPUT number
    IF number % 2 == 0 THEN
        PRINT Even
    ELSE
        PRINT Odd
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> I[/Get input N/]
    I --> B{N % 2 == 0 ?}
    B -->|Yes| C[/Print Even/]
    B -->|No| D[/Print Odd/]
    C --> E([End])
    D --> E([End])
```

---

## 2. Calculate Total and Average Marks

Write the algorithm and draw the flowchart for a program that inputs
marks for 3 subjects, calculates the total and average, and displays
both.

### ✔ Pseudocode

```text
START
    INPUT marks1, marks2, marks3
    Calculate Toatal: marks1 + marks2 + marks3
    Calculate Average: Total/3
    PRINT Total and Average
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/"Enter marks1, marks2, marks3"/]
    B --> C["total = marks1 + marks2 + marks3"]
    C --> D["average = total / 3"]
    D --> E[/"Display Total and Average"/]
    E --> F([End])
```

---

## 3. Display Multiplication Table

Create an algorithm and flowchart that input a number and display its
multiplication table from 1 to 10 using a loop.

### ✔ Pseudocode

```text
START
    INPUT a number N
    SET count = 1
    REPEAT 10 TIMES
        result = N * count
        PRINT result
        count = count + 1
    ENDREPEAT
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/"Enter/Input a number N"/]
    B --> C[count = 1]
    C --> D{"Is count <= 10?"}

    D -- Yes --> E[Calculate: result = N * count]
    E --> F[/"Display num × count = result"/]
    F --> G[count = count + 1]
    G --> D

    D -- No --> H([End])
```

---

## 4. Positive, Negative, or Zero Check

Write the algorithm and flowchart to input a number and display whether
it is positive, negative, or zero.

### ✔ Pseudocode

```text
START
    INPUT a number N
    IF N==0
        PRINT Zero
    ELSE IF N>0
        PRINT Positive
    ELSE
        PRINT Negative
    ENDIF

END

```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/"Enter a number N"/]
    B --> C{"Is N == 0?"}

    C -- Yes --> D[/"Display 'Zero'"/]
    D --> H([End])

    C -- No --> E{"Is N > 0?"}
    E -- Yes --> F[/"Display 'Positive'"/]
    F --> H

    E -- No --> G[/"Display 'Negative'"/]
    G --> H
```

---

## 5. Simple Interest Calculator

Create an algorithm and flowchart for a program that calculates simple
interest using the formula:

**SI = (P × R × T) / 100**

- **P = Principal** → original amount of money
- **R = Rate of Interest** → percentage per year
- **T = Time** → number of years

### ✔ Pseudocode

```text
START
    INPUT Principal amount P
    INPUT Rate of int R
    INPUT Time in year T
        SI = (PxRxT)/100
        DIPLAY SI
END

```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/"Enter Principal amount P"/]
    B --> C[/"Enter Rate of Int R"/]
    C --> D[/"Enter Time in years T"/]
    D --> E["SI = (P × R × T) / 100"]
    E --> F[/"Display Simple Interest"/]
    F --> G([End])

```

---

## 6. Average Temperature Calculation

Write the algorithm and draw the flowchart for a program that takes the
temperature of 7 days, finds the average temperature, and displays it.

```text
START
    SET total = 0, day = 1
    REPEAT 7 TIMES
        INPUT temperature for day (day)
        total = total+temperature
        day = day+1
    ENDREPEAT
        average = total/7
        PRINT average

END

```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[total = 0
                    day = 1]
    B --> C{"Is day <= 7?"}

    C -- Yes --> D[/"Enter temperature for day (day)"/]
    D --> E[total = total + temperature]
    E --> F[day = day + 1]
    F --> C

    C -- No --> G[average = total / 7]
    G --> H[/"Display average temperature"/]
    H --> I([End])

```

---

## 7. Calculate Area of a Rectangle

Create an algorithm and flowchart to input length and width, calculate
the area (**Area = Length × Width**), and display the result.

### ✔ Pseudocode

```text
START
    INPUT the lengt L
    INPUT the width W
        area = L x W
        DIPLAY the area
END

```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/"Enter length L"/]
    B --> C[/"Enter width W"/]
    C --> D["area = L × W"]
    D --> E[/"Display area"/]
    E --> F([End])

```

---

## 8. Determine Pass or Fail

Write the algorithm and draw the flowchart for a program that takes a
student's average marks and displays **"Pass"** if average ≥ 50,
otherwise **"Fail"**.

### ✔ Pseudocode

```text
START
    INPUT student's average marks A
    IF average > = 50
        DIPLAY "Pass"
    ElSE
        Display "Fail"
END

```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/"Enter the student's average marks"/]
    B --> C{"Is average >= 50?"}

    C -- Yes --> D[/"Display 'PASS'"/]
    D --> E([End])

    C -- No --> F[/"Display 'FAIL'"/]
    F --> E

```

---

## 9. Calculate Factorial of a Number

Write the algorithm and draw the flowchart that input a number and
calculate its factorial using a loop.

---

## 10. Calculate Discount on Purchase

Write the algorithm and draw the flowchart for a program that inputs the
purchase amount and gives a **10% discount** if the amount is greater
than 1000.

---
