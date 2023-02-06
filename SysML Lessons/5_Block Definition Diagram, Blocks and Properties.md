# Block Definition Diagrams (BDD)

A Block Definition Diagram is a static structural diagram that shows system components, their contents (Properties, Behaviors, Constraints), Interfaces, and relationships.

*Lesson 5 reading: SysML Distilled - A Brief Guide to the Systems Modeling Language 1st Edition Chapter 3 Block Definition Diagrams*

## Purpose and Use

- BDD: Express information about a system's structure
- BDD model elements: blocks, actors, value types, constraint blocks, flow specifications, & interfaces
  - Elements that appear on a BDD = elements of definition
- BDDs display the structural relationships among elements of definition

### BDD Frame

- The BDD frame
  - Diagram kind abbreviation:bdd
  - Model elements type that the diagram frame represents: package, model, model library, view, block, constraintBlock
  - Model element the diagram represents: namespace (model element that contains other model elements)


    ![BDD Frame](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/BDD%20Lesson%20-%20BDD%20Frame.svg)

## Use of Block Features

- Elements of Definition vs. Elements of Usage (reference Lesson 4 Tables)
  - Definition of types
    - Notation: name only
      - DesktopWorkstation
  - Usage (instances) of types
    - Notation: name and type; separate by colon
      - S3_bucket : S3
- Block: basic unit of structure in SYSML
  - Represents a type of entity, not an instance
- Block notation: rectangle with stereotype <<block>> preceding the name in the name compartment

    ![Block](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/BDD%20Lesson%20-%20block.svg)

### Part Properties


### Reference Properties


### Value Properties



### Constraint Properties



### Ports



#### Standard Ports and Interfaces



#### Flow Ports




##### Nonatomic Flow Ports


##### Atomic Flow Ports


### Operations



### Receptions



## Use of Associations Relationships


### Reference Associations



### Composite Relationships



## Use of Generalization Relationships



## Dependency Relationships



## Use of Actors



## Use of Value Types



## Use of Constraint Blocks



## Use of Comments


## Default Multiplicities





