> I will walk through some of the most basic yet crucial commands you will encounter when starting out with the Terminal.

## Objectives

- Understand what the Terminal is
- Understand the importance of the Unix philosophy and how it relates to programming
- Use fundamental Terminal commands to navigate and manipulate the file structure

```
$ echo "Hello World" >> HelloWorld.txt
$ cat HelloWorld.txt | say
```


## The Command Line Interface

The Command Line Interface (CLI) is a human-computer interface that relies on text inputs and output.

![The terminal](https://s3-us-west-1.amazonaws.com/stanleycyang-v2/Terminal.png-513031f6e74b7ae025f217c21535f9716ec9babd)
*The Command Line Interface on a Macbook*

`This means you can type in commands and your computer will execute them!`


### The Unix philosophy

> Write programs that do one thing and do it well. 

The Command Line Interface (CLI) follows this philophy. The commands you use will be very self-contained and executes on its purpose in the most effective manner.


### Opening the CLI

You can access your Terminal on a `Macintosh` by:
	
- Pressing `Command + Spacebar`
- Type in `terminal`
- Press `<enter>`


### Basic commands

|Command|Meaning|
|---|---|
|pwd|print working directory|
|cd|change directory|
|ls|list|
|touch|creates a file|
|rm|remove|
|mkdir|make directory|
|rmdir|remove directory|
|mv|move|
|man|user manual|


### Getting started

In your terminal now, type the following:

**Note**: *The **$** stands for the beginning of input in the terminal. You do not type the $*

```bash
$ cd ~
$ pwd   
$ mkdir TheAwesomeTutorial
$ cd TheAwesomeTutorial
$ touch stanley is cool
$ ls -l
$ mv * ..
$ cd ..
$ ls
$ rm -rf TheAwesomeTutorial stanley is cool
```

### The results

![The steps](https://s3-us-west-1.amazonaws.com/stanleycyang-v2/tutorial.png-ecc043168f210d04c9277f42c4754c63e2344be4)
*What it looks like in my terminal*

### Understanding what happened

1. We changed to the home directory, in my case it's `/Users/stanley`. The `~` denotes `home`.
2. The `pwd` command printed the current working directory (`/Users/stanley`).
3. We created a new directory called `TheAwesomeTutorial` with the `mkdir` command.
4. Within `TheAwesomeTutorial` directory, we create 3 files called `stanley`, `is`, `cool`, respectively.
5. With the `ls -l` command, we were able to get a detailed list all the files within this directory.
6. We moved all files (The `*` is a wildcard, it'll match everything) to the directory above (denoted by `..`).
7. We changed to a directory above the current, again with `..`.
8. We then removed the directory and the 3 files with the `rm -rf` command. The `-rf` stands for recursive with force, which is dangerous when deleting because it's gone forever.


### At this point in time..

You are now a practioner of the terminal. Regardless of whether you become a programmer or just want to be more efficient on a computer, these skills will translate to all parts of your life if you become fluent.


### Continuing your personal development

Here are some great resources for getting started with the Terminal:

- [Command Line Primer](http://lifehacker.com/5633909/who-needs-a-mouse-learn-to-use-the-command-line-for-almost-anything)
- [Basic Unix](http://mally.stanford.edu/~sr/computing/basic-unix.html)