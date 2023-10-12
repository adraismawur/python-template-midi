❗❗ Replace this readme with a description of your project as soon as possible ❗❗

# python-template-mini
Hi! This is an intermediate template for Python projects. 
The main purpose of this template is to introduce you to structuring your code like a package, and managing requirements.
However, it is not intended to teach you how to write good code. 
That part is up to you :)


### Python templates

|        | link | Focus                             |
|:------:|:----:|-----------------------------------|
| 🐍     | [Mini](https://github.com/adraismawur/python-template-mini) | File and code structure           |
| 🐍🐍   | [Midi](https://github.com/adraismawur/python-template-midi) | Requirements and packaging        |
| 🐍🐍🐍 | [Maxi](https://github.com/adraismawur/python-template-maxi) | Testing, Automatic formatting and checks   |


### Table of contents:

- [Quick start](#quick-start)
- [Why should I use this?](#why-should-i-use-this)
- [What is included in this repository?](#what-is-included-in-this-repository)

## Quick start:

### Prerequisites

❗ This template assumes you are familiar with the concepts explained in the [Mini template](https://github.com/adraismawur/python-template-mini)

❗ Furthermore, this template assumes you are somewhat familiar with:

- Pip, the python package manager (included with Python)

### Set up the repository (local only)

❕Choose this if you are just starting out, or if you do not want to create a page on Github for your code.

1. On this GitHub page, click the **Code** dropdown button in the top-right
2. Click Download ZIP
3. Extract the files somewhere in a new directory
4. Open a shell in the directory where you have extracted the files
5. Edit the readme file to describe your project
6. Run `git add .` to stage all files
7. Run `Git commit -m "initial commit"` to make your first commit

### Set up a remote repository (on GitHub)

❕Choose this if you want to ensure your code is always saved online, or if you want to share your code.

1. Create a new repository of your own by pressing the green button in the top right named "use this template" -> Create a new repository.
   Or [click here](https://github.com/new?template_name=python-template-mini&template_owner=adraismawur)
2. Give your repository a nice name and description
3. Choose whether you want the repository to be public (anyone can see your code), or private.
4. Press "Create repository"

You will be taken to your own github repository page after a few seconds.
From here, you can make edits directly to your files, but it is more practical to download your repository to your local device. (cloning)

1. On your github repository page, click the green button with the text "Code" in the top-right
2. Copy the URL that starts with ```git@github.com:```
3. On your device, open a terminal and navigate to a folder where you want your project to be stored
4. Use the command ```git clone [git url from step 2]```

Your repository will now appear in the folder you navigated to in step 3

### Start coding!

Generally, it is recommended to have the starting point of your code in a file with the name `main.py` inside a folder with the name `your_project_name`.
In there, the `main()` function calls all other functions from separate folders (called modules).

Things to consider while you do so:

✅ Commit early, commit often  
✅ Aim for ~300 lines of code max for a python file  
✅ You do not have to use the template/ subfolder if you have only a few functions/files  
✅ Have fun!  


## Why should I use this?

This template is intended to give you a nice start in managing the elements that your code depends on (requirements), and teaches you how to package your code.
These elements will help you in the future if you want to make an application that is downloadable and installable by other people.

## What is included in this repository?

- Everything that is included in the [Mini repository](https://github.com/adraismawur/python-template-mini)
  - A [README](#a-readme-file) file
  - A (copyleft) [license](#a-license)
  - A basic [folder structure](#folder-structure)
  - A .gitignore file
- A pyproject.toml file
- A requirements.txt file

### Requirements (requirements.txt)

When you write code, you will likely use external libraries to do certain tasks that are either complex, or you do not want to re-implement.
Examples include [numpy](https://numpy.org/) for numerical computing, [pandas](https://pandas.pydata.org/) for numerical computing / data analysis and scikit for machine learning.

Anything your code depends on that is not part of your code or of the standard libraries included in Python, is a _dependency_. The set of _dependencies_ needed to run your code form the code's _requirements_.

To make your code reproducible on other machines, it is important to store:

- What dependencies are needed
- What version of those dependencies are needed

It is important to store both these bits of information, as different versions of dependencies can have different capabilities, and may not work the same as the version that was used when your project was developed.

### Packaging (pyproject.toml)

Packaging is a broad term that involves the process of bundling your software and making it available to other people through distribution using some packaging system.

Your software might not end up as a package that will be installed by other people, but the packaging capabilities of python's built in package manager help in describing your software and making it runnable from the command line if people choose to use your software in that way.
