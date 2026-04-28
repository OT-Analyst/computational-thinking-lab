
# 🧠 Exercise 5: Bottle Deposits

In many jurisdictions a small deposit is added to drink containers to encourage people to  recycle them. In one particular jurisdiction, drink containers holding one liter or less have a $0.10 deposit, and drink containers holding more than one liter have a $0.25 deposit.
Write a program that reads the number of containers of each size from the user. Your program should continue by computing and displaying the refund that will be received for returning those containers. Format the output so that it includes a dollar sign and two digits to the right of the decimal point.

## 1. Problem
> Create a programme that determines the refund a user will recieve for recycled bottles. The refund is based on the volume of the container / bottle and the number of bottles the user deposits.

---

## 2. Inputs
- Quantity / number of bottle(s) returned.
- Volume / Size of the bottle(s) returned.

---

## 3. Validation
- Value types for both quantity and size.
- Number of bottle(s).
- Size of bottle(s).

---

## 4. Process
- User provides the number of bottles <= 1 litre they are returning.
- User provides the number of bottles > 1 litre they are returning.
- Calculate refund based on rate per bottle size.

---

## 5. Output
- Display the refund for recycling the bottles / containers.

---

## 6. Pseudo Code
```
Prompt user for the number of bottles/containers less than or equal to 1 litre returned
Prompt user for the number of containers more than 1 litre returned
Try:
   convert both inputs to integer
   number of bottles less than or equal 1 litre * rate($0.10)
   number of bottles greater than 1 litre * rate($0.25)
   return total_refund rounded off to, 2 decimal places
Except ValueError:
   return error message
```
---

## 7. Test Cases

| Input(s) | Expected Output | Actual Output | Notes |
|----------|-----------------|---------------|-------|
| 1; 3     | $0.85           | $0.85           
| 2; a     | ValueError      | ValueError
| 23;"45"  | ValueError      | ValueError
| 2.3; 2   | ValueError      | ValueError
| 10; 3    | $1.75           | $1.75

---

## 8. Reflection
- What worked?:
I broke down the problem effectively and understood the overall goal: calculate the refund based on bottle categories and quantities, and display the correct total. I had a clear picture of what the final output should look like, which helped guide the solution.

- What didn't work?: 
In the Inputs and Validation sections, I incorrectly treated “bottle size” as something the user would provide. But the problem defines only two fixed categories (≤ 1 litre and > 1 litre), so size is a rule, not an input. This shows I didn’t fully separate problem constraints from user inputs, which affected how I thought about validation and whether a function was needed. It also created inconsistencies between my sections.

- What did I learn?: 
Even with a problem‑solving framework, I can still let small misunderstandings slip through. My sections (Problem → Inputs → Validation → Process → Pseudo Code → Code) didn’t align perfectly, which means I sometimes move forward before confirming that each step logically follows from the previous one. This is a sign that I need to slow down and check my reasoning more deliberately.

- What would I improve next time?:
 Before writing pseudo code or touching Python, I will re‑read through all the sections, prior to the pseudo code section, to make sure they align and accurately reflect the problem. Only once those sections align will I move on. This will help ensure that the pseudo code becomes a direct translation of a well‑understood problem, rather than a place where I fix earlier misunderstandings.
