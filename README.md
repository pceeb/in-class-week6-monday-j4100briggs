## In class exercise

1. If you wanted to reuse this program for a file that had 17 headers lines. What line of code
would you change in our program?

        Write the line of code that you will replace here: if LineNumber > 0

        What will be the new code? The new code will skip over the first 17 lines instead of the first line

        Write the new code here: if LineNumber > 16

2. would happen if we don’t included `import sys` in our program?

        Write you answer here: All the commands that contain the sys program would not work. This includes the sys.argv command.

3. Let’s suppose that the third file that the user provides as input
has only one column. What error message will be generated?

        Write you answer here: Line 1 not XY format in file 3_

4. Our program split lines of input files (except the first file) into elements
that are tab delimitated. However, data could be split by `,` or many other
characters. In this case is a good idea to define a new variable that takes the delimiter
provide by the user. Using what you learn about `sys.argv` in this class`.
Write a variable that reads a delimiter (e.g ',') provided as the first input file.

        Write your code here: add a variable (chosenDelimiter = $1) in the beginning that the user could input as the delimiter, then replace the code containing line.split with the following:
		else:
                    ElementList = Line.split(chosenDelimiter)
                    if len(ElementList) > 0:
                        MasterList[RecordNum] += (chosenDelimiter + ElementList[1]) # += adding instead of replacing
                        RecordNum += 1
				
