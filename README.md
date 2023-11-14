![logo](img/logo.png)
# &nbsp; Orchid  
  
![commit](https://img.shields.io/github/last-commit/erfajo/orchidfordynamo)
![commit activity](https://img.shields.io/github/commit-activity/y/erfajo/orchidfordynamo)
[![license](https://img.shields.io/badge/License-CC%20BY--ND%204.0-yellow)](http://creativecommons.org/licenses/by-nd/4.0/)  
Orchid is a solution designed for use in the [Dynamo](http://dynamobim.org) environment. The solution is designed to support practical, technical, geometrical, logical, and mathematical issues. The solution contains functions to solve data handling in Revit projects, Revit families, and materials in Revit. Besides this, also functions to solve common data handling like geometry, printing, exporting, and system actions. Orchid is among the largest and most coherent solutions besides what Autodesk releases for Dynamo.  
  
**Software environment:**  
Built for Dynamo 2.19 (Revit 2024), Dynamo 2.16 (Revit 2023), Dynamo 2.12 (Revit 2022), and Dynamo 2.6 (Revit 2021).  
  
**Orchid Samples:**  
In the [samples](Samples) folder are examples using the Orchid package placed.  
  
**History/Change Log:**  
Check the [change log](changeLog.md) to see the history of the Orchid package.  
  
---
## Install or Update the package for Dynamo  
Download the **[OrchidForDynamo](Builds/OrchidForDynamo.exe)** executable installer in the [Builds](Builds) folder to install the Orchid package. Likewise if needed, download the [OrchidSamples](Builds/OrchidSamples.exe)  executable installer for the sample collection, and download the [data files](Builds/OrchidSampleDataFiles.exe) for the sample collection.
  
<span style="color:red">**REVIT AND DYNAMO MUST BE CLOSED DURING INSTALLATION!**</span>  
</br>

### Manually installation
The Orchid package may also be installed by manually copying files from the **[Zipped](Zipped)** folder. This is only recommendable for experienced users! To install/update this way, please unzip the zip-file of the chosen version into your dynamo package folder, into a folder named **Orchid**. Download may be handled either by downloading a single file, or by cloning or zipping the repository. The package folder path can be found in Dynamo via the menu item 'Settings' -> 'Manage Node and Package Paths'.  
  
Select the zip-file according to your dynamo version!  
Orchid_219_? &nbsp;&nbsp;&nbsp; (for the dynamo 2.19.x branch)  
Orchid_216_? &nbsp;&nbsp;&nbsp; (for the dynamo 2.16.x branch)  
Orchid_212_? &nbsp;&nbsp;&nbsp; (for the dynamo 2.12.x branch)  
Orchid_206_? &nbsp;&nbsp;&nbsp; (for the dynamo 2.6.x branch)  
Orchid_203_? &nbsp;&nbsp;&nbsp; (for the dynamo 2.3.x branch, however archived and not maintained!)  
Orchid_200_? &nbsp;&nbsp;&nbsp; (for the dynamo 2.0.x branch, however archived and not maintained!)  
  
The individual version is avalible both for the sandbox version and for the version used Inside revit.  
?_Revit &nbsp;&nbsp;&nbsp; (the Revit version)  
?_Core &nbsp;&nbsp;&nbsp; (the Sandbox version)  
  
### Error handling
If Orchid dosnt work after installation, then try to see if you have one of these [errors](Error.md)!  
  
---
## Node description and organization  
Nodes are generally arranged in four node assemblies depending the version. Two assemblies cover the Revit version and two assemblies cover the Core (Sandbox) version. Each of the two sets of assemblies has an assembly for base/standard nodes and an assembly for extensible nodes, mainly dropdown nodes. Besides these four, are assemblies covering external applications outside Revit and icons for the nodes present.  
The nodes may also be used as textual scripted functions in code blocks and custom nodes, example when using design script in code blocks as the Dynamo functions.  
  
Inside Dynamo is the Orchid package nodes arranged into different main branches: Common, RevitFamily, RevitMaterial, RevitProject, About, and Applications. The last branch covers functions for external applications outside Revit. The first four branches covers functions to be used inside Revit. the About branch cover nodes for information about the Orchid package.  
  
Nodes in the four Revit driven branches can be recognized by their icon ribbon/edge color:  
Core -> yellow &nbsp;|&nbsp; RevitFamily -> blue &nbsp;|&nbsp; RevitMaterial -> green &nbsp;|&nbsp; RevitProject -> red  
  
---
## License  
Copyright(c) 2014  
Erik Falck Jørgensen  
  
All content in this repository is part of the Orchid package.  
  
[![license](https://i.creativecommons.org/l/by-nd/4.0/88x31.png)](http://creativecommons.org/licenses/by-nd/4.0/)  
  
This work is licensed under the [Creative Commons Attribution-NoDerivatives 4.0 International](http://creativecommons.org/licenses/by-nd/4.0/) license (CC BY-ND 4.0).  
  
In short terms does the CC BY-ND license state: This license allows for redistribution, commercial and non-commercial, as long as it is passed along unchanged and in whole, with credit to the author.  
  
In the event of violation of the license terms or any other harassment (including, of the author), it will block for the use of the Orchid solution for the user/company until a solution is found.  
