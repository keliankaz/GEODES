# GEODES

Short coding course. 

## Useful resources:

### Conda

In a nutshell conda is here to save you from you. 

Conda creates a 'closed' ecosystem and manages the versions of different softwares and, in particular for this course, python packages that could other conflict with each other. 

When you downloaded conda, you installed a bunch of usefull packages (and a bunch of versions thereof) on your conputer which conda neatly tucks away. Conda gives you a base environment - DON'T USE IT! Alway create a new one. Meanwhile everytime you want version x.y.z because you saw some random post on the internet saying you can solve all your problems with some swanky package they wrote which breaks everything (trust me this will happen) all you will have to do is create a new environment. 

Cheat sheet: https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf

Glossary: https://docs.conda.io/projects/conda/en/latest/glossary.html

The standard workflow when starting a prject is to **always** create a new environment.

For windows:

```
conda create --name MY_GREAT_NEW_PROJECT
activate MY_GREAT_NEW_PROJECT
conda install jupyter numpy matplotlib
````

For mac/linux:
```
conda create --name MY_GREAT_NEW_PROJECT
conda activate MY_GREAT_NEW_PROJECT
conda install jupyter numpy matplotlib
```

The new environment should now show up as one of the interpreters in vscode before running a script or notebook.

If you are working from terminal and want to run a specific file, you can: 

or for windows:
```
activate MY_GREAT_NEW_PROJECT
python this_great_script.py
```


For mac/Linux
```
conda activate MY_GREAT_NEW_PROJECT
python this_great_script.py
```

### VScode

VScode is an IDE. You know how there are 10 different softwares to look at PDFs. IDEs are basically that, but for text files and coding. VScode is a very very fancy text editor. If you are develloping code in python make sure to peruse the extensions (little blocks on the left-hand column of tools for python specific extensions). 

https://code.visualstudio.com/docs/getstarted/getting-started

### python

There are tons of python tutorials out there. Substack is a great resources, more and more, ChatGPT or Claude are becoming increadible resources. 

These resources are crutches. Use them sparingly and make sure you know exactly what is going in your code.

### Conding best practices

Read this if you are doing research!

https://carpentries-lab.github.io/good-enough-practices/index.html

I try to follow the following style guide:
https://google.github.io/styleguide/pyguide.html#

### Version control: git and github

We do not cover this in the short course, but it is best to get in the habit of using version control. 

https://education.github.com/git-cheat-sheet-education.pdf

The most common workflow will be (in the terminal):
```
git init

...make changes...

git add FILENAME
git commit -m "added new things"
```

Note that vscode has very nice version control tools available as extension. 