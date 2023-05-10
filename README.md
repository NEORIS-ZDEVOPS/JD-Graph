# JD Graph Extension for z/OS

**Job Discovery Graph Extension for z/OS. It's an extension for Visual Studio Code that speeds up JCL jobs development and execution.**

This extension has been designed to help developers to have a global view of the JCL files they work with. It paints a graph with the selected job at the center. The central node's parents are the dependencies and the children are the dependents.

## Features

- Draws a graph with job relations.
- Allows opening a graph from the context menu of a workspace file.
- Can execute jobs and notifies when the job has ended.
  - Has the option to set-up environment variables in jcl files with the following formats:
    - Scheduler style "%%variable.".
    - XML style "\<Variable\>".
    - JSON style "{variable}".
- Checks if required DataSets are present before execution.
- Allows exporting the graph to a SVG file.

## Requirements

- To use this extension it is required an extraction process of the current scheduler's data.
- To use the z/OS connection capabilities, it is required to have configured a ZOWE profile. A ZOWE profile, in turn, requires the mainframe to have "zosmf" or "rse api".

## Extension Settings

- Connection details to z/OS.
- Configuration details of where to find the extracted scheduler's data (USS or MVS allowed).
- Job execution policies.
  - Environment variables declaration.
  - Default Environment.
  - Enable/Disable datasets checking.

## Known Issues

- Datasets existence validation before job execution can fail if the dataset is created within same job. (You can disable datasets checking for this case until we deploy the fix.)

Soon a link will be provided with an issue tracker.

## How to use

We have plans to create a public repository to provide the know-hows. As soon as it will be available, we will provide the link.