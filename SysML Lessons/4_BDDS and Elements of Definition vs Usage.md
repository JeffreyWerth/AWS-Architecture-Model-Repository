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
- Block notation: rectangle with stereotype <<<block>>> preceding the name in the name compartment

    ![Block](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/BDD%20Lesson%20-%20block.svg)

## Element of Definition

The term definition refers to a model element that is a classifier or type such as a block. The element is defined by specifying its features such as the properties and operations of a block. The term usage identifies a defined element in a particular context; for now I want you to understand this concept on this lesson, bellow are some examples.

The elements in the BDD are **elements of definition** while the elements in the IBD are **elements of usage**.

Elements of Definition
- Block is a definition/type
- Captures properties, etc
- Reused in multiple contexts

| Elements of Definition: |       | Elements of Usage:                                                                                                 |
| ----------------------- | ----- | ------------------------------------------------------------------------------------------------------------------ |
| Actor                   | types | Reference Property or Lifeline                                                                                     |
| Block                   | types | Part Property, Reference Property, Lifeline, Atomic Flow Fort, Flow Property, Object Node, or Constraint Parameter |
| Value Type              | types | value Property, Constraint Parameter, Atomic Flow Port, Flow Property, or Object Node                              |
| Constraint Block        | types | Constraint Property                                                                                                |
| Flow Specification      | types | Noatomic Flow Port                                                                                                 |
| Signal                  | types | Atomic Flow Port, Flow Property, or Object Node                                                                    |
| Interface               | types | Atomic Flow Port, Flow Property, or Objet Node                                                                     |
| Association             | types | Connector                                                                                                          |
| Activity                | types | Call Behavior Action                                                                                               |
| Interaction             | types | Call Behavior Action                                                                                               |
| State Machine           | types | Call Behavior Action                                                                                               |


Elements of Usage
- Part is the usage in the context of a composing block
-Also known as a role


| Elements of Usage:                                |       | Elements of Definition:                 |
| ------------------------------------------------- | ----- | --------------------------------------- |
| Part Property                                     | types | Block                                   |
| Reference Property                                | types | Block or Actor                          |
| Value Property                                    | types | Value Type                              |
| Constraint Property                               | types | Constraint Block                        |
| Constraint Parameter                              | types | Value Type, Block                       |
| Nonatomic Flow Port                               | types | Flow Specification                      |
| Atomic Flow Port                                  | types | Block, Value Type, or Signal            |
| Standard Port                                     | types | Interface                               |
| Flow Property                                     | types | Block, Value Type, or Signal            |
| Connector                                         | types | Association                             |
| Call Behavior Action                              | types | Activity, Interaction, or State Mahcine |
| Object Node (includes Pin and Activity Parameter) | types | Block, Value Type, or Signal            |
| Lifeline                                          | types | Block or Actor                          |

