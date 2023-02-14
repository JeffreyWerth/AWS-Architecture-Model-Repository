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

- Standard Ports 
    - (most often) Displayed as a small square straddling the border of a block
    - Can have a modeler defined name
    - Can have one or more types
    - Types are the interfaces assigned        ![Standard Port]()
- Interfaces
    - Element of definition
  - Defines a set of operations and receptions that clients and providers will conform to      ![Interface Block]()
    - Assigned as either a provided interface or a required interface
        - Provided interface is displayed with the ball notation
        - A block that provides an interface must implement all of the interface’s operations and receptions
        - Required interface is displayed using the socket notation
        - A block that requires an interface may invoke one or more of it’s operations and receptions (but not necessarily all)

            ![Ports]()

### Flow Ports

- (most often) Displayed as a small square straddling the border of a block and a symbol inside the small square
          ![Flow Ports]()
- Can have a modeler defined name and type; name and type shown as a string floating near the flow port
    - Format = < name> : < type>
- Two types of flow ports: nonatomic and atomic

#### Nonatomic Flow Ports

- Symbolized as <>: multiple types of items can flow in and out of that port
- Typed by a flow specification defined somewhere in the system model
- Flow specification- element of definition; defines a set of flow properties that can flow in or out of nonatomic flow port
          ![Flow Specification]()
- Flow property- specific item that can flow in or out of a block via a flow port (has a direction, name, and type)
    - Notation = < direction> < name> : < type>
        - Direction can be in, out, inout
        - Name is modeler defined
        - Type is a value type, block, signal created somewhere in the system model
- Conjugated (~): directions of the flow properties are reversed

#### Atomic Flow Ports

- Symbolized as an arrow conveying direction of flow
- Single type of item can flow in or out via that port
          ![Atomic Flow Ports]()
- Type is a value type, block, or signal created somewhere in the system model

## Operations

- Behavior that a block performs when a client calls it; invoked by a call event
    - Most often synchronous, but doesn’t have to be
- Displayed in the operations compartment of a block
    - Notation = < operation name> (< parameter list>) : < return type> [< multiplicity>]
        - Operation name is modeler defined
        - Parameter list: comma separated list of parameters
            - Parameters: inputs or outputs of the operation
            - Parameter notation: < direction> < parameter name> : < type> [< multiplicity>] = < default value>
                - Direction: in, out, inout
                - Parameter name is modeler defined
        - Type: value type or block created somewhere in the system model     ![Operations]()
                - Multiplicity: constraint on the number of instances of the type that the parameter can represent
                - Default value: value assigned to the parameter if no value is specified as an argument when the operation is called
        - Return type: value type or block created somewhere in the system model
        - Multiplicity: # of instances of the return type the operation can return to the caller when it completes
- Good practice: use a verb phrase to name an operation (it’s a behavior!)

## Receptions

- Behavior that a block performs when a client sends a signal that triggers it; invoked by a signal event
    - Always represents an asynchronous behavior
- Signal: can represent any type of matter, energy, data that one part of a system sends to another part
    - Signals can own properties (ex. Data carried from client to target)
    - Signal properties become inputs to the reception
    - The client can add values for properties to the instance of a signal
    - The reception must have a parameter with a compatible type for each property of the signal
- Reception notation: << signal>> < reception name> (< parameter list>)
    - Reception name must match the name of the signal that triggers it
  - Parameter notation: < parameter name> : < type> [< multiplicity>] = < default value> ![Receptions]()
        - Parameter name is modeler defined
        - Type: value type or block that exists somewhere in the system model
        - Multiplicity: constraint on the number of instances of the type that the parameter can represent
        - Default value: value assigned to the parameter if no value is provided in the corresponding property of the signal
- Receptions cannot have return types (b/c they are asynchronous)
    - Parameters can only be inputs and never outputs


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





