### Exercise: Area of a room
Write a program that asks the user to enter the width and length of a room. Once these values have been read, your program should compute and display the area of the room. The length and the width will be entered as floating-point numbers. Include units in your prompt and output message; either feet or meters, depending on which unit you are more comfortable working with.

#### Problem solving framework:
Problem:
> A programme that calculates the area of a room, with input provided by user.

Inputs:
> User provide dimensions - length and width.

Validation:
> Inputs provided are numeric.

Process:
> Create a function that calculates the area of a room.
> Prompt user to provide dimensions in prefered units of measure.
> Insert user dimensions in function.

Output:
> Display the area of the room

#### Pseudo Code:
Define function area (<i>width, length</i>) :</br>
&emsp;Try:
&emsp;&emsp;SET width = float(width)</br>
&emsp;&emsp;SET length = float(length)</br>
&emsp;&emsp;SET area = width * length</br>
&emsp;&emsp;return area</br>
&emsp;Except ValueError:</br>
&emsp;&emsp;Display: "Invalid input! width and length must be numbers."</br>
</br>
SET width_input = "Enter the width of a room"</br>
SET length_input = "Enter the length of a room"</br>
SET result = area(user_input)</br>
Display: Total area: {measure} square metres</br>
