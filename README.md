# odMLtablesForMNG

## Introduction
Metadata is essential for sharing data according to FAIR principles. Standards are well established for most electrophysiological recording methods, but are still lacking in microneurography. We propose a standard for structuring and recording metadata based on [odML](http://g-node.github.io/python-odml/) and [odML-tables](https://github.com/INM-6/python-odmltables) by providing two templates for experimental properties adapted to microneurography recordings and installation guidelines to ensure usability. In addition, we present an extension to the odML-tables GUI, in which we integrate a new search functionality for a large database adapted to our needs. With our open-source repository, we encourage all microneurography labs to incorporate odML-based metadata into their lab routines. 

## Templates
There are two [templates](https://github.com/Digital-C-Fiber/odMLtablesForMNG/tree/master/Templates). One for general experimental metadata and the other one for individual data recordings. Please take a look at the filled out [example templates](https://github.com/Digital-C-Fiber/odMLtablesForMNG) or check out the [github wiki](https://github.com/Digital-C-Fiber/odMLtablesForMNG).

## Installation 
1. Get the most recent version of **python** from https://www.python.org, and download **git** from https://git-scm.com/downloads. 
2. Start setup of python installation and make sure python.exe is added to the path by selecting the checkbox "Add python.exe to PATH". <br>
![grafik](https://user-images.githubusercontent.com/14880611/210798277-42707e62-6e82-4cf4-8aea-6b5271094b7a.png)
3. Start setup of git installation. 

4. Open the **Command Line** window for windows or **Terminal** for linux/macOS.

5. Install pipx - a program manager for python:
	- Type into command line or terminal and press enter:
	```console
	python -m pip install pipx
	```
6. Install odmltables:
	```console
	pipx install odmltables
	```
7. Now the standard version of odML-tables was installed. To add the new search functionality, certain files need to be downloaded and used as replacement for the old files. 
	1. Download and save the python files in the same hierarchical structure. For example, click on green button **<> Code** and select "Download ZIP".<br>
	2. Navigate to folder where pipx is installed and odmltables is located, for that write in command line or terminal
	```console
	pipx list
	```
	3. It should show: <code>venvs are in YOURPATH\\.local\pipx\venvs</code> <br>
	Navigate to the folder location in your file system by replacing YOURPATH with your actual path<br>
	<code>YOURPATH\\.local\pipx\venvs\odmltables\Lib\site-packages\odmltables</code>
8. Copy and replace files from [Code folder](https://github.com/Digital-C-Fiber/odMLtablesForMNG/tree/master/code)
	1. Copy [odml_table.py](https://github.com/Digital-C-Fiber/odMLtablesForMNG/tree/master/code/odml_table.py) to folder <code>YOURPATH\\.local\pipx\venvs\odmltables\Lib\site-packages\odmltables</code>
	2. Copy [mainwindow.py](https://github.com/Digital-C-Fiber/odMLtablesForMNG/tree/master/code/gui/mainwindow.py) to folder <code>YOURPATH\\.local\pipx\venvs\odmltables\Lib\site-packages\odmltables\gui</code> (in gui folder).
	3. Copy [searchpages.py](https://github.com/Digital-C-Fiber/odMLtablesForMNG/tree/master/code/gui/searchpages.py) to folder <code>YOURPATH\\.local\pipx\venvs\odmltables\Lib\site-packages\odmltables\gui</code> (in gui folder).
	4. Copy [searchwiz.py](https://github.com/Digital-C-Fiber/odMLtablesForMNG/tree/master/code/gui/searchwiz.py) to folder <code>YOURPATH\\.local\pipx\venvs\odmltables\Lib\site-packages\odmltables\gui</code> (in gui folder).
	5. Copy [searchodml3.svg](https://github.com/Digital-C-Fiber/odMLtablesForMNG/tree/master/code/gui/graphics/searchodml3.svg) to folder <code>YOURPATH\\.local\pipx\venvs\odmltables\Lib\site-packages\odmltables\gui\graphics</code> (in gui/graphics folder).
	
	
## Problems or questions
If you observe any problems or questions in this extension of odML-tables please add a issue at the [GitHub issue tracker](https://github.com/Digital-C-Fiber/odMLtablesForMNG/issues).


## Publication to cite
Please cite the following [publication](https://pubmed.ncbi.nlm.nih.gov/37697832/): Troglio A, Nickerson A, Schlebusch F, Röhrig R, Dunham J, Namer B, Kutafina E. odML-Tables as a Metadata Standard in Microneurography. Stud Health Technol Inform. 2023 Sep 12;307:3-11. doi: 10.3233/SHTI230687. PMID: 37697832.
