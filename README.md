# odMLtablesForMNG

## Introduction
Metadata is essential for sharing data according to **FAIR principles**. Standards are well established for most electrophysiological recording methods, but are still lacking in microneurography. 

This repository provides a metadata workflow for microneurography recordings based on **[odML](http://g-node.github.io/python-odml/)** and **[odML-tables](https://github.com/INM-6/python-odmltables)**.

The repository contains:

- metadata **templates** for microneurography experiments  
- a **user manual (PDF)** describing the metadata workflow  
- a **standalone executable** of the odMLtables GUI with additional search functionality  
- links to the **modified odMLtables repository** used in this workflow  

The goal is to provide an easy-to-use metadata standard that can be integrated into everyday lab routines and support **FAIR data management in microneurography research**.

---

## Repository Contents

### Templates
Two metadata templates are provided in the **[Templates](https://github.com/Digital-C-Fiber/odMLtablesForMNG/tree/master/Templates)** folder:

- **Experiment template** – general experimental metadata  
- **Recording template** – metadata for individual microneurography recordings  

---

### User Manual

The **manual (PDF)** explains the complete workflow, including:

- how to fill out the metadata templates  
- how to convert templates to odML format  
- how to merge metadata into the central database  
- how to search and explore metadata using the GUI  

---

### Executable (GUI)

A **standalone executable** of the odMLtables graphical user interface is provided in this repository.

This version includes an **extended search wizard** that allows:

- searching for specific terms in metadata  
- searching for **property–value pairs**  
- interactive exploration of large metadata collections  

This functionality was developed to facilitate exploration of larger microneurography metadata databases.

---	

## Modified odMLtables Software

The modified odMLtables version used in this workflow is maintained in a separate repository:

**[odMLtables fork with search functionality](https://github.com/Digital-C-Fiber/python-odmltables)**

The fork extends the original GUI with the **Search Wizard** used in this metadata workflow.

---

## Installation

### Option 1 - Use the executable (recommended)

Download the executable from this repository and start the GUI directly.

No Python installation is required.


### Option 2 - Install from the modified odMLtables repository

If you prefer installing the software via Python, you can install the modified version directly from the GitHub repository:

```bash
pip install git+https://github.com/Digital-C-Fiber/python-odmltables
```
---

## Problems or questions
If you observe any problems or questions in this extension of odML-tables please add a issue at the [GitHub issue tracker](https://github.com/Digital-C-Fiber/odMLtablesForMNG/issues).

---
## Publication to cite
If you use this workflow or templates in scientific work, please cite this [publication](https://pubmed.ncbi.nlm.nih.gov/37697832/): 

Troglio A, Nickerson A, Schlebusch F, Röhrig R, Dunham J, Namer B, Kutafina E. odML-Tables as a Metadata Standard in Microneurography. Stud Health Technol Inform. 2023 Sep 12;307:3-11. doi: 10.3233/SHTI230687. PMID: 37697832.

---
## Contact
Email: alina.troglio@rwth-aachen.de
