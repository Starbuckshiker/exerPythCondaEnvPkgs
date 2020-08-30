# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [ ] Fork this repository so you have your own copy to work on.
- [ ] Clone the repository on your local machine. 
- [ ] Edit this README.md file on your machine.
- [ ] Run the Conda commands shown in the video and describe them in the table below.
- [ ] Push your changes to your GitHub repository.
- [ ] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/N6806_Fall2020_DevNotes/blob/master/Projects/002%20-%20Practice%20Using%20Git%20and%20GitHub/README.md
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.
  
## Edit your README.md file

* [ ] In an editor of your choice (i.e. VSCode) edit this README.md file to add the answers requested in the tables.

## Follow along with this tutorial

* Conda What and Why? (27 min): https://www.youtube.com/watch?v=23aQdrS58e0&list=PLG9A6ovzPqX6d9uWzx0UYN9pm0zzl5ofA&index=13&t=0s
  * He installs Miniconda. We will be using Anaconda. Don't install Miniconda.
  * Follow along with the rest of the tutorial.
  * Go ahead and create the environments as he creates them in the tutorial.

## Conda Concepts

* [ ] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |(lets the user specific environment for a specific application)|
|What is the default package manager in Python?            |(pip-)|
|How do you manage environments and packages in Anaconda?  |(virtualenv or Anaconda/ MiniConda)|
|`conda list`       |(Shows you all the packages and versions installed in an active enviroment )|
|`conda env list`       |(shows you all your environments)|
|How do you keep your base environment unchanged?       |(enter description or short answer here)|
|What is the link to the Conda cheat sheet? (link in video notes is broken)      |(https://www.youtube.com/redirect?event=video_description&v=23aQdrS58e0&redir_token=QUFFLUhqbWhZWFBybnJJaHZzc0ZKMDVlZmo1aGtHaE1FZ3xBQ3Jtc0trM3dnX0kyNXpPZ1JRZXZqa2pfZVl0X0s0NVJselByWFZwM2JKWW9IajM2NW13MHRSbXV6QmZDOUVxb3UtMXJLVWhfcHQzODZhZlR3SFl0RkJIZkFvQ0JBdWF4aGozeVUweVpwV01vN1M5QUl5cmlYUQ%3D%3D&q=https%3A%2F%2Fconda.io%2Fdocs%2F_downloads%2Fconda-cheatsheet.pdf)|

|`conda create --name XXXX`       |(conda create --name py35 python=3.5)|
|`source activate XXXX`       |(source activate py35)|
|`conda install YYYY`       |(conda install --reversion 2)|
|channels in Conda       |(tells conda to look for the packaage else where)|
|`conda install -c ZZZZ YYYY`       |(you can install different packages in the different enviroments)|
|`conda config --show channels`       |(shows you the channels you have)|
|`conda config --add channels ZZZZ`       |(you can add additional channels to find/ install the package you are looking for)|
|conda-forge.org       |(highest priority channel)|
|`source deactivate`       |(to switch or go back to base channel)|
|`conda config --get channels`       |(allows you to look at the level of priority )|

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
base                     C:\Users\dlist\anaconda3
ai37                     C:\Users\dlist\anaconda3\envs\ai37
da35                  *  C:\Users\dlist\anaconda3\envs\da35


```
* What command would you use to remove the environments you created for this exercise from your computer?

```
conda env remove --name [Name(s) of env to remove]

```
