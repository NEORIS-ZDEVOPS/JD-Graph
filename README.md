# Scheduler Viewer Extension for z/OS

**Scheduler Viewer Extension for z/OS is an extension for Visual Studio Code that helps with JCL jobs development and execution.**

This extension has been designed to help developers to have a global view of the JCL files they work with. It paints a graph with the selected job at the center. The central node's parents are the dependencies and the children are the dependents.

## Features

- Draws a graph with job relations.
- Allows opening a graph from the context menu of a workspace file.
- Can execute jobs and notifies when the job has ended.
  - Has the option to set-up environment variables in jcl files with the following formats:
    - Scheduler style "%%variable.".
    - XML style "\<variable\>".
    - JSON style "{variable}".
    - JS string interpolation style "${variable}".
- Checks if required DataSets are present before execution.
- Allows exporting the graph to a SVG file.

## Requirements

- To use this extension it is required an extraction process of the current scheduler's data.
- To use the z/OS connection capabilities, it is required to have configured a ZOWE profile. A ZOWE profile, in turn, requires the mainframe to have "zosmf" or "rse api".

## Known Issues

Issues can be checked in the [issue tracker](https://github.com/NEORIS-ZDEVOPS/JD-Graph/issues)

## How to use

Check the documentation in [our github page](https://github.com/NEORIS-ZDEVOPS/JD-Graph/tree/master/doc)