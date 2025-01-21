## Lab Assignment 1 - Shell

**Due**  - Saturday, 1 March, by midnight

**This project is to be done individually.**

**Tests** - Under `./shell/tests`

### Notes

The basic project description is found in `./shell/README.md`. Please read this carefully in order to understand exactly what to do.

There's a modification to that basic description:

1. There is a special built-in command you need to add, which is called **loop**. When the user types:

	```
	prompt> loop 10 somecommand
	```

	the wish shell should run `somecommand` ten times.
	For example, if the user types `echo hello` as the command (to run the program `/bin/echo` , which just prints out whatever the arguments to it are), the shell should do this:

	```
	prompt> loop 5 echo hello
	hello
	hello
	hello
	hello
	hello
	prompt>
	```
    To make this slightly more useful, there is one more feature you'll need to add, a loop variable. This variable is referred to by `$loop `. Thus, the user should then be able to do type:

	```
	prompt> loop 5 echo hello $loop
	hello 1
	hello 2
	hello 3
	hello 4
	hello 5
	prompt>
	```

### Handing In Submission

The code has to be sumbitted via your repository on GitHub Classroom. Your code should be in a single file `wish.c`, which we will compile and test on the same set of test cases provided to you. 

The responsibility to ensure that you've pushed your changes to the Classroom repository, and not just committed to your local repo, lies with you.
