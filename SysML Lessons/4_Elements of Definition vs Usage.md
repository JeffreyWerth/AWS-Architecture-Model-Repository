# Element of Definition

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
| Object Nide (includes Pin and Activity Parameter) | types | Block, Value Type, or Signal            |
| Lifeline                                          | types | Block or Actor                          |

