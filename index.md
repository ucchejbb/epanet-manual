# EPANET Manual

Water Infrastructure Division
Center for Environmental Solutions and Emergency Response
Office of Research and Development
U.S. Environmental Protection Agency
Cincinnati, OH 45268 
 
## Disclaimer

This User Manual is an updated version of the EPANET 2 Users Manual
(EPA/600/R-00/057) written by Lewis Rossman in 2000. The EPANET 2 software
was developed by the United States Environmental Protection Agency (EPA).

EPANET Version 2.2 includes contributions from EPA and individuals outside
the United States Government. It has been subjected to review by the Office of Research and Development and approved for publication. Approval does not signify that the contents reflect the views of the Agency, nor does mention of trade names or commercial products constitute endorsement or recommendation for use. 

Execution of any EPANET installation program, and modification to system configuration files must be made at the user's own risk. Neither the U.S. EPA nor the program author(s) can assume responsibility for program modification, content, output, interpretation, or usage.

EPANET installation programs have been extensively tested and verified. However, as for all complex software, these programs may not be completely free of errors and may not be applicable for all cases. In no event will the U.S. EPA be liable for direct, indirect, special, incidental, or consequential damages arising out of the use of the programs and/or associated documentation.




## EPANET 2.2 User Manual Overview
[Introduction](docs/1_introduction.md) of this manual describes what EPANET is and its
capabilities.

[Quick Start](docs/2_quickstart.md) describes how to install EPANET and offers
up a quick tutorial on its use. Readers unfamiliar with the basics of
modeling distribution systems might wish to review [Network Models](docs/3_network_model.md)
first before working through the tutorial.

[Network Model](docs/3_network_model.md) provides background material on how EPANET
models a water distribution system. It discusses the behavior of the physical
components that comprise a distribution system as well as how
additional modeling information, such as time variations and
operational control, are handled. It also provides an overview of how
the numerical simulation of system hydraulics and water quality
performance is carried out.

[Workspace](docs/4_EPANET_workspace.md) shows how the EPANET workspace is organized. It
describes the functions of the various menu options and toolbar buttons, and
how the three main windows – the Network Map, the Browser, and the
Property Editor—are used.

[Projects](docs/5_projects.md) discusses the project files that store all of the
information contained in an EPANET model of a distribution system. It
shows how to create, open, and save these files as well as how to set
default project options. It also discusses how to register
calibration data that are used to compare simulation results against
actual measurements.

[Objects](docs/6_objects.md) describes how one goes about building a network
model of a distribution system with EPANET. It shows how to create the various
physical objects (pipes, pumps, valves, junctions, tanks, etc.) that
make up a system, how to edit the properties of these objects, and
how to describe the way that system demands and operation change over
time.

[Map](docs/7_map.md) explains how to use the network map that provides a
graphical view of the system being modeled. It shows how to view
different design and computed parameters in color-coded fashion on
the map, how to re-scale, zoom, and pan the map, how to locate
objects on the map, and what options are available to customize the
appearance of the map.

[Analyzing Network](docs/8_analyzing_network.md) shows how to run a hydraulic/water quality
analysis of a network model. It describes the various options that control how
the analysis is made and offers some troubleshooting tips to use when
examining simulation results.

[Viewing Results](docs/9_viewing_results.md) discusses the various ways in which the
results of an analysis can be viewed. These include different views of the
network map, various kinds of graphs and tables, and several different types
of special reports.

[Printing/Copying](docs/10_printing_copying.md) explains how to print and copy the views
discussed in [Viewing Results](docs/9_viewing_results.md).

[Importing/Exporting](docs/11_importing_exporting.md) describes how EPANET can import and
export project scenarios. A scenario is a subset of the data that characterizes
the current conditions under which a pipe network is being analyzed
(e.g., consumer demands, operating rules, water quality reaction
coefficients, etc.). It also discusses how to save a project’s entire
database to a readable text file and how to export the network map to
a variety of formats.

[Questions](docs/12_questions.md) answers questions about how EPANET can be used
to model special kinds of situations, such as modeling pneumatic tanks,
finding the maximum flow available at a specific pressure, and
modeling the growth of disinfection by-products.

[Analysis Algorithms](docs/analysis_algorithms.md) provides details of the procedures and
formulas used by EPANET in its hydraulic and water quality analysis algorithms.


The manual also contains several appendixes.

 - [Units](docs/A_units.md) provides a table of units of expression for all design and computed parameters.
 - [Error Messages](docs/B_error_messages.md) is a list of error message codes and their meanings that the program can generate.
 - [Command Line](docs/C_command_line_EPANET.md) describes how EPANET can be run from a command line prompt within a DOS window, and discusses the format of the files that are used with this mode of operation.

