# AppianMerger

## Background
Exporting and Deployment of Appian Objects requires the UUID or DataType Namspace to be included in the application XML file.
Without the UUID or the DT Namespace, the application will not be able to list the objects. 

## Objective
To reduce manual work for scanning of application XML file for existing UUID or DT Namespace of exported Appian objects. 
To insert the UUID of the exported objects into the respective object groups if the UUID doesn't exist.

## MacOS/Linux Usage
```bash
./appianMerger <Path of Object Directory> <Path of Application XML>

./appianMerger <Path of Object Directory> <Path of Application XML> [Options...]
```
### Example
```bash
./app ~/Downloads/Patch_2018 ~/Documents/appian-package/bgp-app/application/_a-0000db0e-a3c0-8000-0315-010000010000_2041.xml
```

## Windows Usage
```bash
appianMerger.exe <Path of Object Directory> <Path of Application XML>

appianMerger.exe <Path of Object Directory> <Path of Application XML> [Options...]
```
### Example
```bash
app.exe c:/Downloads/Patch_2018 ~/Documents/appian-package/bgp-app/application/_a-0000db0e-a3c0-8000-0315-010000010000_2041.xml
```

|Arguments|Description|
|:-----------------------|:---|
|Path of Object Directory|Path of Unzipped Directory of exported Appian Objects which contains objects folders|
|Path of Application XML|Path of checked out Application XML file eg.appian-package/bgp-app/application/_a-0000db0e-a3c0-8000-0315-010000010000_2041.xml|

|Options|Description|
|:-----------------------|:---|
|-t|Only Check for Existing or Missing Objects in the Application. No change to application XML|

### References
* [TinyXML2] (http://www.grinninglizard.com/tinyxml2/) C++ XML Library
* [MinGW] (http://www.mingw.org) C++ Compiler for Windows

## Happy Coding :thumbsup:




