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
- Notation = < part name> : < type> [multiplicity, 1..1]

    ![Part Property](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/BDD%20Lesson%20-%20Part%20Properties.svg)


- Multiplicity: constraint on the number of instances that the part property can represent within the composite
    - Expressed as a single integer OR a range of integers
    - Unconstrained number of instances: [ 0..*] or [ *]
    - If no multiplicity is shown for a part property, the default is 1; [ 1..1]

## Reference Properties

- Represents a structure that is external to the block
- Does NOT convey ownership (i.e. it’s an external structure); represents a “needs” relationship
    - implies some type of connection must exist
- Notation = < reference name> : < type> [multiplicity, 1..1]
    - Typed by a block or actor somewhere in the system model
- Multiplicity: constraint on the number of instances that the reference property can represent within the composite
    - Expressed as a single integer OR a range of integers
    - Unconstrained number of instances: [ 0..*] or [ *]
    - If no multiplicity is shown for a reference property, the default is 1; [ 1..1]

    ![Reference Property]()

## Value Properties

- Represents a quantity, a Boolean, or a string (often- something you assign a number to)
- Notation = < value name> : < type> [multiplicity, 1..1] = < default value>
    - Typed by a value type somewhere in the system model
    - < default value> is optional

    ![Value Properties]()

- Multiplicity: constraint on the number of instances that the value property can represent within the composite
    - Expressed as a single integer OR a range of integers
    - Unconstrained number of instances: [ 0..*] or  [ *]
    - If no multiplicity is shown for a value property, the default is 1; [ 1..1]
    - Value property referred to as a collection when it’s multiplicity has an upper bounder greater than 1
- Can hold values that are both assigned or derived (calculated)
    - A forward slash (/) in front of the value name conveys value property is derived

    ![Value Properties]()

## Constraint Properties

- Represents a mathematical relationship that is imposed on a set of value properties
- Notation = < constraint name> : < type>
  - Typed by a constraint block somewhere in the system model
    - constraint blocks generally encapsulate mathematical equations
  
    ![Constraint Properties]()

- Blocks can own constraint properties to constrain value properties

## Ports

- Represents a distinct interaction point at the boundary of a structure through which external entities can interact with that structure – to:
    - Provide or request a service
    - Exchange matter, energy, or data
- Decouples a block’s clients from any particular internal implementation
- Can represent any type of interaction point
    - Physical object (fuel nozzle, HDMI jack)
    - Software object (message queue, GUI)
    - Interaction between business organizations (purchase order, website)
- Two kinds of ports (v1.2 and earlier)
    - Standard port: specify the interaction with a focus on services that a block provides or requires
    - Flow port: specify an interaction with a focus on types of matter, energy, or data that can flow in and out of a block

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





