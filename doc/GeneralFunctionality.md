# General functionality<a id="general-functionality"></a>

## Table of contents<a id="table-of-contents"></a>
- [General functionality](#general-functinality)
	- [Table of contents](#table-of-contents)
	- [Introduction](#introduction)
	- [Set Up](#previous-settings)
	- [Open a graph](#open-a-graph)
		- [Open a Graph from json](#open-a-graph-from-json)
			- [Open from this](#open-from-this)
			- [Open default](#open-default)
			- [Load graph data](#load-graph-data)
		- [Open a graph from jcl](#open-a-graph-from-jcl)
	- [Movement in the graph](#movement-in-the-graph)
	- [Zoom in/out](#zoom-inout)
	- [Highlight path](#highlight-path)
	- [Hide path](#hide-path)
	- [Show path](#show-path)

## Introduction<a id="introduction"></a>
In this section, we explain the overall operation of the application.

## Set Up

Before explaining the extension's functionalities, it is necessary to configure a series of parameters for proper operation.

1. **Used Zowe Profile:**
	For all operations related to Zowe, it is necessary to establish the Zowe profile to use.
	![gif featuring load zowe profile](./assets/ZoweProfile.gif)
	
	1.1. Go to zowe explorer section.
	1.2. Right click button on the desire profile to select(rse, zosmf)
	1.3. Click on the "Set Scheduler Viewer ZOWE profile"
	**Note:** Can put the profile manually from Settings -> Extensions -> Scheduller Viewer -> Used Zowe Profile and introduce the desired profile.  
	<br>
2. **Default graph file**
	A default file must be selected for default graph file, are two types:
	1. **Zowe Default File Path**
		It will selected if the Use USS option is checked. It will obtain the file from Unix System Services.
	![gif featuring Zowe default path](./assets/UssFilePath.gif)
		2.1.1 Go to Settings -> Extensions -> Scheduller Viewer
		2.1.2 Check the Use USS option
		2.1.3. Introduce the path for Zowe Default File Path
	<br>
	2. **Local Default File Path**
		This path will selected if the Use USS option is not checked.
		![gif featuring Local File default path](./assets/LocalFilePath.gif)
		2.2.1 Go to Settings -> Extensions -> Scheduller Viewer
		2.2.2 Uncheck the Use USS option
		2.2.3 Introduce the path for Local Default File Path
		**Note:** Relative paths are relative to the project.

### Open a Graph
Are two ways to open a Graph, from a .json or .jcl files.

**Note**: Opening a graph will only be possible if a default file path is configured, either for a local file or a Zowe file

#### Open a Graph from json<a id="open-a-graph-from-json"></a>

**Prerequisite**: Having a default path configured.

Note: We have several ways to open or load a file from json.

##### Open from this
**Prerequisite**: Having a .json file opened

![gif featuring open from this graph](./assets/OpenFromThis.gif)

1. With the .json file opened, press Ctrl + shift + p
2. Select "Scheduler Viewer: Open From This" 
##### Open default
**Prerequisite**: A default path configured
![gif featuring open default graph](./assets/OpenDefault.gif)

1. With the .json file opened, press Ctrl + shift + p
2. Select "Scheduler Viewer: Open Default"

##### Load Graph data

![gif featuring load graph data](./assets/LoadGraphData.gif)

1. Press Ctrl + shift + p
2. Select "Scheduler Viewer: load Graph Data"

#### Open a graph from jcl<a id="open-a-graph-from-jcl"></a>
**Prerequisite**: Having a default path configured and .jcl file accesible on explorer section.
![gif featuring open jcl data](./assets/OpenJclGraph.gif)
1. Right click bottom on a .jcl file(Explorer section)
2. Select "Open in default graph" option

### Movement in the graph<a id="movement-in-the-graph"></a>

![gif featuring load graph](./assets/MovementRedone.gif)

Prerequisite: Having a graph loaded

1. Click and hold the left mouse button, then drag the graph to move it across the canvas.

### Zoom in/out<a id="zoom-inout"></a>

![gif featuring load graph](./assets/ZoomRedone.gif)

Prerequisite: Having a graph loaded

1. Scroll the mouse wheel to zoom in or out.

### Highlight path<a id="highlight-path"></a>

![gif featuring load graph](./assets/Path.gif)

Prerequisite: Having a graph loaded

1. Click in a node.
2. Display the path to the main node.

### Hide path<a id="hide-path"></a>

![gif featuring hide path](./assets/HidePath.gif)

1. Click on minus icon below the node.

### Show path<a id="show-path"></a>

![gif featuring hide path](./assets/ShowPath.gif)

1. Click on plus icon below the node

