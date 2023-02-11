# Error handling  
  
One thing there will course an error is. If Revit is running while installing, then will it work the first time Orchid is installed (after a restart of Dynamo), next time Orchid is being "upgraded" while Dynamo is running or has been started and Revit is still running, then will it fail. This is due to applications in Windows environment read the needed assemblies (DLL files) when the application is opened. Windows will then protect these files from being changed unless they explicitly are unprotected. Unprotecting files could course other unintended issues and this is why Dynamo and Revit need to be closed during the installation of Orchid.  
Do always ensure Revit (and Dynamo) is closed during installation!  
  
### Dynamo package path  
The executable installer will install Orchid in the first given path in Dynamo menu item  
<i><ins>before</ins> Dynamo 2.10 --></i> 'Settings' -> 'Manage Node and Package Paths'  
<i><ins>from</ins> Dynamo 2.10 --></i> 'Dynamo' -> 'Preferences' -> 'Package Manager'  
If you want to move the default location for packages, then put the path you want to use as the first path. This may also include network and unc paths!  
  
### Dynamo default path <ins>from</ins> 2.10 versions  
From Dynamo version 2.10 has the dynamo team included a first path for "Dynamo Built-In Packages" in Dynamo menu item 'Dynamo' -> 'Preferences' -> 'Package Manager' there is related to the given Dynamo version. This will course that Orchid will be installed by its version! ...meaning an Orchid 212 will be installed in a 2.12 packages path even if it is installed in a Dynamo 2.10 version, and might not be loaded due to this!  
This can be solved by adding the needed path manually or by moving the Orchid package manually.  
  
### Errors coursed by improper packages 
If a package is shipped including Dynamo assemblies, then will packages fail if dependencies for a specific version of Dynamo exist in the package. Orchid is written for specific versions due to the enormous scope of Orchid. This kind of error happens on rare occasions, however, if it happens, it seems to be if package builders are new to coding and the community. They might not know that this will involve unintended behavior in Dynamo. All packages should be shipped without any Dynamo assemblies, let Dynamo handle its assemblies. All serious packages are shipped without Dynamo assemblies.  
This can usually be ascertained by moving all other packages out of the package path so that nothing but Dynamo works, and then moving package by package back... starting with Orchid, since this will let you know that it works!  
  
### Errors coursed by the IFC Exporter 
Orchid nodes for the IFC Exporter is also version-specific. Please ensure that you are using the latest released version for your Revit version. The latest IFC Exporter that can be found at
[github.com/Autodesk/revit-ifc](http://github.com/Autodesk/revit-ifc).  
  
### Errors coursed by Windows  
A well-known "error" is windows blocking files upon download, and this includes the executable, the zipped file, and the assembly files in the package. Files that are meant to place in system folders like %ProgramData% and %AppData% may be blocked by Windows to protect the system, if so, then unblock the files, by entering the 'Properties' -> 'Unblock' menu item.  
![unblock](img/unblock.png)  
  
### Other challenges  
In the last couple of years have many things changed in Revit, old methods change names and functions, new methods arrive, and some methods are being deprecated. Also, Dynamo is concurrently being developed which in itself involves challenges.  
However, the largest challenge is the development of the Orchid package. The package is constantly expanding and the amount of new methods is huge. This involves challenges for the organization of nodes in the package, which are being reorganized when there is no other way around to keep the progress of Orchid development.  
