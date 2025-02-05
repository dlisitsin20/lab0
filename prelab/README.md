# ECE 281 Lab 1 Prelab

## Prelab questions

### Truth Table

| A | B | C | D | Y |
|---|---|---|---|---|
| 0 | 0 | 0 | 0 | X |
| 0 | 0 | 0 | 1 | 1 |
| 0 | 0 | 1 | 0 | 0 |
| 0 | 0 | 1 | 1 | 1 |
| 0 | 1 | 0 | 0 | 0 |
| 0 | 1 | 0 | 1 | 1 |
| 0 | 1 | 1 | 0 | 0 |
| 0 | 1 | 1 | 1 | 1 |
| 1 | 0 | 0 | 0 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 0 | 1 | 1 | 0 |
| 1 | 1 | 0 | 0 | 1 |
| 1 | 1 | 0 | 1 | X |
| 1 | 1 | 1 | 0 | X |
| 1 | 1 | 1 | 1 | X |

### Boolean Equation

$$
Y = A'D+AD'
$$

### Digital Simulations

In this folder are also Digital templates for you to complete and simulate.  Do not change the file names or the input and output labels in Digital otherwise the autograder will not work.  The autograder will look in the prelab folder for the files.

Complete all three circuits using the various approaches (generic multiplexer symbol, 74151 multiplexer chip, and a sum of products using and/or logic gates).

You may also wish to run test cases.  The first two rows of the truth table have been added to the Digital simulation files as a test.  You may wish to edit the test to add more rows and fully cover all possible cases but this is not required.

## Submission

1. Make sure all prelab files are in this folder
2. Commit all files
3. Push to GitHub
4. Submit to Gradescope
5. Verify submission

Documentation Statement: C2C Payton Nunn helped me with drawing the MUX by hand by explaining that I could
rearrange the truth table so that output is represented by one of the variables. C3C Cody Goth helped me with Digital MUX 74154
by helping me rearrange my truth table to make A the MSB. C3C Jillian Essig helped me with my KMap by explaining that the circle 
can only be drawn including other circles if it is needed to include a 1 that is not included in any other circle. https://stackoverflow.com/questions/12258399/how-do-i-create-a-folder-in-a-github-repository
<- used that website to try to create a folder for the KMap, until I understood that prelab/kmap ment a file name not a folder.
https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository 
<- needed this to delete the lab branch so I can start over because I can't push because of the folder I added. Great, I couldn't delete it and now it's stuck in a merge I don't know how to finish.