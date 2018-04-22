# Introduction
## Purpose
This subsection should:

1. Delineate the purpose of the SRS;
1. Specify the intended audience for the SRS.

## Scope 
This subsection should:

1. Identify the software product(s) to be produced by name (e.g., Host DBMS, Report Generator, etc.);
1. Explain what the software product(s) will, and, if neceflary, will not do;
1. Describe the application of the software being specified, including relevant benefits, objectives, and goals;
1. Be consistent with similar statements in higher-level specifications (e.g., the system requirements specification), if they exist.

##  Definitions, acronyms, and abbreviations

This subsection should provide the definitions of all terms, acronyms, and abbreviations required to properly interpret the SRS. This information may be provided by reference to one or more appendixes in the SRS or by reference to other documents.

## References
This subsection should

1. Provide a complete list of all documents referenced elsewhere in the SRS;
1. Identify each document by title, report number (if applicable), date, and publishing organization;
1. Specify the sources from which the references can be obtained.
 
 This information may be provided by reference to an appendix or to another document.
 
## Overview
This subsection should

1. Describe what the rest of the SRS contains;
1. Explain how the SRS is organized.

# Overall description
This section of the SRS should describe the general factors that affect the product and its requirements. This section does not state specific requirements. Instead, it provides a background for those requirements, which are defined in detail in Section 3 of the SRS, and makes them easier to understand.

This section usually consists of six subsections, as follows:
   
1. Product perspective;
1. Product functions;
1. User characteristics;
1. Constraints;
1. Assumptions and dependencies;
1. Apportioning of requirements.

## Product Perspective
This subsection of the SRS should put the product into perspective with other related products. If the product is independent and totally self-contained, it should be so stated here. If the SRS defines a product that is a component of a larger system, as frequently occurs, then this subsection should relate the requirements of that larger system to functionality of the software and should identify interfaces between that system and the software.

A block diagram showing the major components of the larger system, interconnections, and external interfaces can be helpful.

This subsection should also describe how the software operates inside various constraints. For example, these constraints could include

1. System interfaces;
1. User interfaces;
1. Hardware interfaces;
1. Software interfaces;
1. Communications interfaces;
1. Memory;
1. Operations;
1. Site adaptation requirements.

## Product Functions
This subsection of the SRS should provide a summary of the major functions that the software will perform.

For example, an SRS for an accounting program may use this part to address customer account maintenance, customer statement, and invoice preparation without mentioning the vast amount of detail that each of those functions requires.

Sometimes the function summary that is neceflary for this part can be taken directly from the section of the higher-level specification (if one exists) that allocates particular functions to the software product.

Note that for the sake of clarity:

1. The functions should be organized in a way that makes the list of functions understandable to the customer or to anyone else reading the document for the first time.
1. Textual or graphical methods can be used to show the different functions and their relationships. Such a diagram is not intended to show a design of a product, but simply shows the logical relationships among variables.

## User Characteristics
This subsection of the SRS should describe those general characteristics of the intended users of the product including educational level, experience, and technical expertise. It should not be used to state specific requirements, but rather should provide the reasons why certain specific requirements are later specified in Section 3 of the SRS.

## Constraints
This subsection of the SRS should provide a general description of any other items that will limit the developer’s options. These include:

1. Regulatory policies;
1.  Hardware limitations (e.g., signal timing requirements);
1.  Interfaces to other applications;
1.  Parallel operation;
1.  Audit functions;
1.  Control functions;
1.  Higher-order language requirements;
1.  Signal handshake protocols (e.g., XON-XOFF, ACK-NACK);
1.  Reliability requirements;
1.  Criticality of the application;
1.  Safety and security considerations.

##  Assumptions and dependencies
This subsection of the SRS should list each of the factors that affect the requirements stated in the SRS.

These factors are not design constraints on the software but are, rather, any changes to them that can affect the requirements in the SRS. For example, an aflumption may be that a specific operating system will be available on the hardware designated for the software product. If, in fact, the operating system is not available, the SRS would then have to change accordingly.

# Requirements
## Functional Requirements
### Mode 1
#### External interface requirements
This should be a detailed description of all inputs into and outputs from the software system. It should complement the interface descriptions in IEEE 830-1998 5.2 and should not repeat information there.

It should include both content and format as follows:

1. Name of item;
1. Description of purpose;
1. Source of input or destination of output;
1. Valid range, accuracy, and/or tolerance;
1. Units of measure;
1. Timing;
1. Relationships to other inputs/outputs;
1. Screen formats/organization;
1. Window formats/organization;
1. Data formats;
1. Command formats;
1. End messages

##### User interfaces
This should specify the following:
1. *The logical characteristics of each interface between the software product and its users.* This includes those conÞguration characteristics (e.g., required screen formats, page or window layouts, content of any reports or menus, or availability of programmable function keys) necessary to accomplish the software requirements.

1. *All the aspects of optimizing the interface with the person who must use the system.* This may simply comprise a list of do's and don'ts on how the system will appear to the user. One example may be a requirement for the option of long or short error messages. Like all others, these requirements should be veriÞable, e.g., "a clerk typist grade 4 can do function X in Z min after 1 h of training" rather than Òa typist can do function X. Ó (This may also be speciÞed in the Software System Attributes under a section titled Ease of Use.)

##### Hardware interfaces
This should specify the logical characteristics of each interface between the software product and the hardware components of the system. This includes conÞguration characteristics (number of ports, instruction sets, etc.). It also covers such matters as what devices are to be supported, how they are to be supported, and protocols. For example, terminal support may specify full-screen support as opposed to line-by-line support.

#####  Software interfaces
This should specify the use of other required software products (e.g., a data management system, an operating system, or a mathematical package), and interfaces with other application systems (e.g., the linkage between an accounts receivable system and a general ledger system). For each required software product, the following should be provided:

- Name;
- Mnemonic;
- Specification number;
- Version number;
- Source.

For each interface, the following should be provided:

 - Discussion of the purpose of the interfacing software as related to this software product.
 - Definition of the interface in terms of message content and format. It is not necessary to detail any well-documented interface, but a reference to the document defining the interface is required.

##### Communications interfaces
This should specify the various interfaces to communications such as local network protocols, etc.

#### Functional Requirements
1. Functional Requirements 1
1. Functional Requirement n

#### Performance
### Mode n
## Design constraints
This should specify design constraints that can be imposed by other standards, hardware limitations, etc.

##  Software system attributes
There are a number of attributes of software that can serve as requirements. It is important that required attributes be specified so that their achievement can be objectively verified.

### Reliability
This should specify the factors required to establish the required reliability of the software system at time of delivery.

### Availability
This should specify the factors required to guarantee a defined availability level for the entire system such as checkpoint, recovery, and restart.

### Security
This should specify the factors that protect the software from accidental or malicious access, use, modification, destruction, or disclosure. Specific requirements in this area could include the need to

1. Utilize certain cryptographical techniques;
1. Keep specific log or history data sets;
1. Assign certain functions to different modules;
1. Restrict communications between some areas of the program;
1. Check data integrity for critical variables.
### Maintainability
This should specify attributes of software that relate to the ease of maintenance of the software itself. There may be some requirement for certain modularity, interfaces, complexity, etc. Requirements should not be placed here just because they are thought to be good design practices.
### Portability
This should specify attributes of software that relate to the ease of porting the software to other host machines and/or operating systems. This may include the following:

1. Percentage of components with host-dependent code;
1. Percentage of code that is host dependent;
1. Use of a proven portable language;
1. Use of a particular compiler or language subset;
1. Use of a particular operating system.

##  Other requirements
