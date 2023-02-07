# Use of Block Features Part 2

- Block Features come in two varieties: Structural and Behavioral
- 5 kinds of structural features (aka properties)
    - Part properties
    - Reference properties
    - Value properties
    - Constraint properties
    - Ports
- 2 kinds of behavioral features
- Operations
- Receptions

*Lesson 5 reading: SysML Distilled - A Brief Guide to the Systems Modeling Language 1st Edition Chapter 3 Block Definition Diagrams*

## Part Properties

- Represents a structure that is internal to the block
- Represents ownership (a part property can belong to only one composite structure at a time) 
- ‘typed by’ a “block”
- Notation = <<part name>? : <<type>> [<multiplicity>]

    ![Block](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/BDD%20Lesson%20-%20block.svg)


- Multiplicity: constraint on the number of instances that the part property can represent within the composite
    - Expressed as a single integer OR a range of integers
    - Unconstrained number of instances: [0..*] or [*]
    - If no multiplicity is shown for a part property, the default is 1; [1..1]

## Reference Properties


## Value Properties



## Constraint Properties



## Ports



### Standard Ports and Interfaces



### Flow Ports




#### Nonatomic Flow Ports


#### Atomic Flow Ports


## Operations



## Receptions



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





