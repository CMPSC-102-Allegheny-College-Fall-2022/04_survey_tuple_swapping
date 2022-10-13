# Tuple Swapping

## Assigned: 
## Due: 

## Project Goals

This assignment invites you to run and observe one Python program called
`perform-ordered-pair-swap`. Instead of using the
[Poetry](https://python-poetry.org/) tool for managing dependencies and
packaging these programs, this program is a script, without any dependencies on other Python
packages, that you can run through the Python interpreter. As you continue to
practice a different way to run a Python program, this project invites you to
explore how to (i) find and fix defects in a function and (ii) create and use
fixed-size tuples that can contain arbitrary types of data.

## Project Access

If you are a student enrolled in a Computer Science class at Allegheny College,
you can access this assignment by clicking the link provided to you in Discord.
Once you click this link it will create a GitHub repository that you can clone
to your computer. Specifically, you
will need to use the `git clone` command to download the project from GitHub to
your computer. Now you are ready to add source code and documentation to the
project!

## Code Survey

If you change into the `source` directory of your GitHub repository, you will
see a Python program called `perform-ordered-pair-swap.py`. Your goal for this
project is to find and fix the defects in the function with the signature `def
ordered_pair_swap(pair_one: Tuple[Any, Any], pair_two: Tuple[Any, Any]) ->
Tuple[Tuple[Any, Any], Tuple[Any, Any]]`. When you run the command `python
perform-ordered-pair-swap.py` after correcting the program's defects, it should
produce the following output:

```
Original tuple of ordered pairs: (('A', 1), ('B', 2))
Swapped tuple of ordered pairs: ((2, 'B'), (1, 'A'))
Swapped (again) tuple of ordered pairs: (('A', 1), ('B', 2))
```

It is worth noting that the `ordered_pair_swap` function performs two types of
swapping. It first swaps the values inside of each of the ordered pairs, as
evidenced in the first and second lines of the output, where the first tuple is
input as `('A', 1)` and output as `(1, 'A')`. The second type of swap performed
by the function involves outputting the second tuple first and the first tuple
second, which the second output line illustrating with `((2, 'B'), (1, 'A'))`
for an input of `(('A', 1), ('B', 2))`. The final line of the program output
also illustrates that the tuple swapping process is reversible since the
function can accept as input `((2, 'B'), (1, 'A'))` and produce as output
`(('A', 1), ('B', 2))` &mdash; which is the original tuple that started this the
tuple swapping process!

## Running Checks

Since this project does not use [Poetry](https://python-poetry.org/) to manage
project dependencies and virtual environments, it does not support the use of
commands like `poetry run task test`. However, you can use `gatorgrade --config config/gatorgrade.yml` to check your work. If `gradle grade` shows that all checks pass, you will know that you made progress towards correctly implementing and writing about this project's program.

## Project Reflection

Once you have finished all of the previous technical tasks, you can use a text
editor to answer all of the questions in the `writing/reflection.md` file. Since
this is a source code survey, you should provide output from running each of the
provided Python programs on your own laptop and then explain how the program's
source code produced that output. A specific goal for this project is for you to
improve and document the source code of a function that indexes a tuple in order
to swap its contents.

## Submission

As you are working on your lab, you are to commit and push regularly. The commands are the following.

```bash
git add -A
git commit -m ``Your notes about commit here''
git push
```

After you have pushed your work to your repository, please visit the repository at the GitHub website (you may have to log-in using your browser) to verify that your files were correctly sent.

## Project Assessment

The grade that a student receives on this assignment will have the following components.

- **GitHub Actions CI Build Status [up to 50%]:**: For the lab01 repository associated
with this assignment students will receive a checkmark grade if their last before-the-deadline
build passes. This is only checking some baseline writing and commit requirements as well as correct
running of the program. An additional reduction will given if the commit log shows a cluster
of commits at the end clearly used just to pass this requirement. An addition reduction
will also be given if there is no commit during lab work times. All other requirements are evaluated manually.

- **Mastery of Technical Writing [up to 25%]:**: Students will also receive a checkmark
grade when the responses to the writing questions presented in the `reflection.md` reveal
a proficiency of both writing skills and technical knowledge. To receive a checkmark grade,
the submitted writing should have correct spelling, grammar, and punctuation in addition
to following the rules of Markdown and providing conceptually and technically accurate answers.

- **Mastery of Technical Knowledge and Skills [up to 25%]**: Students will receive a portion
of their assignment grade when their program implementation reveals that they have mastered
all of the technical knowledge and skills developed during the completion of this assignment.
As a part of this grade, the instructor will assess aspects of the programming including,
but not limited to, the completeness and the correctness of the program and the use of
effective source code comments.

## Seeking Assistance

Students who have questions about this project outside of the lab time are invited to ask them in the course's Discord channel or during instructor's or TL's office hours.
