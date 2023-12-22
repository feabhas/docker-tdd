# Feabhas Docker TDD Project

**Contents**
- [Feabhas Docker TDD Project](#feabhas-docker-tdd-project)
- [Getting Started](#getting-started)
- [Exercise solutions](#exercise-solutions)


# Getting Started

Download this git repo to your local machine. If possible you should clone
the repo to your local hard drive and avoid using network attached storage
as the editing and build process is disk I/O intensive.

Avoid placing the folder in an area that is mirrored using OneDrive, 
Google Drive or similar for the same reasons.

Install and then startup VS Code. Use the extension icon (left hand icon
bar) to install the Dev Containers extension from Microsoft. You may need to 
restart VS code after doing this. 

In the bottom left corner of the screen there will now be a green icon with 
an `><` symbol, click on this and select:

   * **Open Folder in container...** 

and open the folder you have just created.

When VS Code opens the folder this will download a Docker container from 
`feabhas/ubuntu-tdd:latest`. This container is configured with a
toolchain for building Feabhas embedded training projects including:

   * Host based GCC GDB
   * Build tools GNU Make and CMake
   * TDD tools

The container is about 3GB and will take a noticeable amount 
of time to download.

VS Code will connect to the remote container as user `feabhas` (password
`ubuntu`) and copy files from an embedded target project template to
the working folder. Within the container the working folder is mapped
onto `~/workspace`.

# Exercise solutions

Download the appropriate GitHub repo for your TDD course. Typically 
this will be one of:

TDDC-301 
   * https://github.com/feabhas/tddc-301_exercises

TDCPP-301
   * https://github.com/feabhas/tddcpp-301_exercises

Clone the exercise repo into the VM working directory and follow the
instructions in the exercise for building the exercises and solutions.
