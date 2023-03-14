# Bash Scripting LAB1

Welcome to the Bash Scripting laboratory. We prepared some exercises to improve your Bash Scripting knowledge.

<br>

## Exercises
<br><br>
Create a script that will ask the following questions:
- What is your first name?
- What is your last name?
- Where were you born?

<br>
And display this output:

 <h3> Nice to meet you <b>"first name" "last name"</b> from <b>"birth place"</b>!
 </h3>

Script:

#!/bin/sh

echo  "What is your first name?"
read fname
echo "What is you last name?"
read lname
echo "Where were you born?"
read born

echo Nice to meet you $fname $lname from $born!