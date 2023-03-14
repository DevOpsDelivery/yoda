# Bash Scripting LAB2

## Exercises
<br><br>
Create a script that will do the following:
- Receive three numbers as input parameters
- Print on stdout if each number is even or odd

<br>
And display this output:

<h3 style="text-align:center">First number is <b>"even or odd"</b></h3>
<h3 style="text-align:center">Second number is <b>"even or odd"</b></h3>
<h3 style="text-align:center">Third number is <b>"even or odd"</b></h3>

Bash :

#!/bin/sh

echo "Please input one number"
read first
echo "Please input a second number"
read second
echo "PLease input a third number"
read third

if [ $((first%2)) -eq 0 ]; then
	echo "First number is even"
else
	echo "First number is odd"
fi

if [ $((second%2)) -eq 0 ]; then
        echo "Second number is even"
else
        echo "Second number is odd"
fi

if [ $((third%2)) -eq 0 ]; then
        echo "Third number is even"
else
        echo "Third number is odd"
fi