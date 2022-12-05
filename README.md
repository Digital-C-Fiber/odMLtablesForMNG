# odMLtablesForMNG

## Introduction
Metadata is essential for sharing data according to FAIR principles. Standards are well established for most electrophysiological recording methods, but are still lacking in microneurography. We propose a standard for structuring and recording metadata based on [odML](http://g-node.github.io/python-odml/) and [odML-tables](https://github.com/INM-6/python-odmltables) by providing a template for experimental properties adapted to microneurography recordings and installation guidelines to ensure usability. In addition, we present an extension to the odML-tables GUI, in which we integrate a new search functionality for a large database adapted to our needs. With our open-source repository, we encourage all microneurography labs to incorporate odML-based metadata into their lab routines. 

## Templates
There are two [templates](https://github.com/Digital-C-Fiber/odMLtablesForMNG). One for general experimental metadata and the other one for individual data recordings. Please take a look at the filled out [example templates](https://github.com/Digital-C-Fiber/odMLtablesForMNG) or check out the [user guidelines](https://github.com/Digital-C-Fiber/odMLtablesForMNG)

### Installation
1. Get a version of python (> 3.9) from https://www.python.org, and download git from https://git-scm.com/downloads. 
2. Install pipx - a program manager for python:
	- Open command line/terminal (Windows key + R) and enter:
	> python -m pip install pipx
4. Install odmltables:
> pipx install odmltables
5. Add search functionality. For that you need to replace python files from [Code](https://github.com/Digital-C-Fiber/odMLtablesForMNG) in the same structure.
	- Navigate to folder where pipx is installed and odmltables is located .local\pipx\venvs\odmltables\Lib\site-packages\odmltables
	Enter in command line
	> pipx list
	It should show: venvs are in YOURPATH\.local\pipx\venvs
	Navigate to the folder location in the windows explorer. 
	
## Problems or questions
