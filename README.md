# Assignment #1

The first assignment is about setting up accounts and your programming
environment.  

> :warning: Do not panic if feel lost! We are going to work with these
>           tools a lot, so, with time, you will become familiar with them.

Here are the steps to get started:

0. Install `git` and `python` on your computer.
   For Linux and Mac, `bash` is built-in.
   For windows, scroll down for more detailed informations.
   We also suggest using [Anaconda](https://www.anaconda.com/products/individual) to get `python` and related packages

1. If you do not have an account on GitHub yet, please
   [register](https://github.com/signup).

2. Then, join the right session in GitHub classroom:

   - [Session 1](https://classroom.github.com/classrooms/97425980-phys-105a-session-1)
   - [Session 2](https://classroom.github.com/classrooms/97425980-phys-105a-session-2)

3. Once you join GitHub classroom, you can accept the assignment by
   clicking:

   - [Session 1](https://classroom.github.com/a/vxHYdJF3)
   - [Session 2](https://classroom.github.com/a/5l3Frsbk)

4. Follow the instruction on GitHub to `clone` your home work
   repository.
   Specifically, if you use command line, you will clone your copy of
   the assignment by

       git clone git@github.com:uarizona-2022spring-phys105a/01-[YOUR_GITHUB_USERNAME].git

   where `[YOUR_GITHUB_USERNAME]` above is your GitHub username, and
   the repository `01-[YOUR_GITHUB_USERNAME].git` was automatically
   generated for you by GitHub Classroom.

5. To actually work on your assignment, go into the
   `01-[YOUR_GITHUB_USERNAME]` directory and edit the text file
   `assignment.py` to print "hello world".
   Hences on how to print strings from python can be found in the
   [hands-on note](https://github.com/uarizona-2022spring-phys105a/phys105a/blob/main/01/Handson.ipynb).

6. Finally, to submit the assigment, you need to add your script back
   to the repository and push it back to GitHub.
   If you use command line, you may use

       cd `01-[YOUR_GITHUB_USERNAME]` # change-directory into the repository
       git add .                      # add changed files to the "index"
       git commit -m 'Finished'       # commit your changes
       git push                       # push to GitHub, i.e., submission
       
## Set up your development environment on Windows

Windows does not come with convenient tools to do develop the software we are
going to build in this class. For this reason, we recommend installing the
"Windows Subsystem for Linux" (WSL). WSL is a Windows package that installs a
small Linux system __inside_ Windows. Once WSL is installed, you will be able to
run programs that are designed for Linux.

### Install WSL

- Update your Windows to the latest version available (Start > Settings > Update
  & Security > Windows Update > Check for updates)
- Open a Windows Command Prompt as administrator (right click, "Run as
  administrator")
- Type "wsl --install"

After WSL is installed, you will see a new Ubuntu app among your installed
applications. The first time you open that you will be asked to create a new
user. You will have to choose a username and a password. Anything is fine, this
user is local to your computer. When you type the password, nothing will show
up: don't panic, this is intended.

Opening the Ubuntu app will launch a terminal in the Linux subsystem. Here, you
can type all the shell commands. For example, you can print the current
directory with `pwd`, or change directory with `cd`. Your Linux subsystem comes
with most of the tools we are going to need, so you can immediately use `git`.
If you want to install a new program you can do it with `apt`. Just type in the
command-line `sudo apt install PROGRAM` and type your password. When you are
working in the command-line, you can use the arrows to navigate back to command
that you executed in the past, and you can use the TAB key to auto-complete
commands and filenames.

You can continue with parts 1-4. Read the section below for part 5 of the
assignment.

### Text editors

You will often have to edit files for your assignments. To do that, you will
need a text editor. The world is full of text editors and you can pick the one
you prefer, but in this context, you will roughly have two choices: install it
on Windows, or on Linux. For example, you can install VSCode or PyCharm on
Windows (as you would install any other program). If you do that, the home
directory of your Linux subsystem lives in /wsl/ubuntu/home/USERNAME/, so you
can navigate to that its subdirectories to edit your files. Alternatively, you
can use a Linux-native text-editor. Popular command-line choices are Emacs, vim,
or nano. These editors tend to be fast and powerful, but the learning curve is
steeper.

Now you can do part 5. Remember, to run your program type `chmod 755
PROGRAM_NAME`, and then execute it with `./PROGRAM_NAME`

### SSH keys

To connect to GitHub, we need a SSH key. In your terminal, type
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```
This will create a new key. Press Enter when asked about the location and the password
(you do not need a password for your SSH key, so you can leave that blank).

Follow
[this](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
tutorial to add your SSH key to your GitHub account.

You are all set!




