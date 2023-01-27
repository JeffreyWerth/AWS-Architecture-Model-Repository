# SysML Language and Diagram Types

To learn more about System Modeling Language, follow the link to the summary lesson on SysML Diagrams (https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/1_SysML%20Diagrams.md).

## Structural Diagrams

The elements in a structure diagram represent the meaningful concepts of a system, and may include abstract, real world and implementation concepts; the following structural diagram are part of the SysML standard:

- Block Definition Diagrams 
- Internal Block Diagrams 
    - Parametric Diagrams mark
- Package Diagrams 

## Block Definition Diagram (bdd)

A Block Definition Diagram is a static structural diagram that shows system components, their contents (Properties, Behaviors, Constraints), Interfaces, and relationships.
• Blocks can be recursively decomposed ("nested") into Parts by alternating between Block Definition Diagram (BDD) definitions and Internal Block Diagram (IBD) usages (See Usage Notes TBD.)
• Behaviors can either be encapsulated by Blocks (e.g., Operations, Signals, and State Machines) or Allocated (via «allocate» Dependency) to Blocks (e.g., Activities/Actions) directly or indirectly (via Interfaces).

The purpose of Block Definition Diagrams is to specify system static structures that be used for Control Objects, Data Objects, and Interface Objects.

To learn more about Block Definition Diagrams, follow the link to the summary lesson on bdd
(https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/5_Block%20Definition%20Diagram%2C%20Blocks%20and%20Properties.md)

## Internal Block Diagram (ibd)

An Internal Block Diagram is a static structural diagram owned by a particular Block that shows its encapsulated structural contents: Parts, Properties, Connectors, Ports, and Interfaces. Stated otherwise, an IBD is a "white-box" perspective of an encapsulated ("black-box") Block.
• Blocks can be recursively decomposed ("nested") into Parts by alternating between Block Definition Diagram (BDD) definitions and Internal Block Diagram (IBD) usages (See Usage Notes TBD.)
• Behaviors can either be encapsulated by Blocks (e.g., Operations, Signals, and State Machines) or Allocated (via «allocate» Dependency) to Blocks (e.g., Activities/Actions) directly or indirectly (via Interfaces).
• Blocks can be mathematically constrained via Constraint Blocks to produce mathematically representations of Parametric diagrams.

The purpose of Internal Block Diagrams (IBDs) is to show the encapsulated structural contents (Parts, Properties, Connectors, Ports, Interfaces) of Blocks so that they can be recursively decomposed and "wired" using Interface Based Design techniques

To learn more about Internal Block Diagrams, follow the link to the summary lesson on ibd
(https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/7_Internal%20Block%20Digrams.md)

### Parametric Diagram (par)

A Parametric diagram is a specialization of an Internal Block Diagram (IBD) that enforces mathematical rules (Constraints) defined by Constant Blocks across the internal Part Value Properties bound in the Constraint Block Parameters.
The purpose of Parametric diagrams (PARs) is to enforce mathematical rules across Block Value Properties.

To learn more about parametric Diagrams, follow the link to the summary lesson on par
(https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/8_Parametric%20Diagrams.md)

## Package Diagram (pkg)

A Package diagram is a static structural diagram that shows the relationships among packages and their contents. Package can be stereotyped (customized) for organizing model elements into models, views, model libraries, and frameworks.
The purpose of Package diagram is to support the organization and management of large, complex System Architecture Models (SAMs).

To learn more about Package Diagrams, follow the link to the summary lesson on pkg
(https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/2_Namespace%20and%20Package%20Diagrams.md)

## Requirement Diagram (req)

A SysML Requirement Diagram is a static structural diagram that shows the relationships among Requirement (<< requirements >>) them, and Test Cases that Verify (<< verify >> Dependency) them. The purpose of Requirement diagrams is to specify both Functional and Non-Functional Requirements within the model so that they can be traced to other model elements that Satisfy them and Test Cases that Verify them.

To learn more about Requirements Diagrams, follow the link to the summary lesson on req
(https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/11_Requirements%20Diagram.md)

## Behavioral Diagrams

Behavior diagrams show the dynamic behavior of the objects in a system, which can be described as a series of changes to the system over time; the following behavioral diagrams are part of the SysML standard:

- Activity Diagram 
- Sequence Diagram 
- State Machine Diagram 
- Use Case Diagram 

## Activity Diagram (act)

An Activity diagram shows system dynamic behavior using a combined Control Flow and Object (data) Flow model.
• Activities (and indirectly Activity diagrams) can be recursively decomposed ("nested") by alternating between Activity definitions and Call Behavior Action usages (See Usage Notes below).
• Activities and Actions can be Allocated (via to Partitions that represent Control Blocks (i.e., Blocks that represent the System, Subsystems, Sub-Subsystems, ..., atomic structures)
• Data Blocks (i.e., Blocks that represent Persistent Data Stores) and Signals that contain Data Blocks can be Allocated to Activity Parameters and Action Pins.

The purpose of Activity diagrams is to specify dynamic system behaviors that Satisfy («satisfy» Dependency) system Functional Requirements using both Control and Object (data) Flows.

To learn more about Acitivity Diagrams, follow the link to the summary lesson on act
(https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/6_Activity%20Diagrams.md)

## Sequence Diagram (seq)

 A Sequence diagram is a dynamic behavioral diagram that shows interactions (collaborations) among distributed objects or services via sequences of messages exchanged, along with corresponding (optional) events.
• collaborating objects or services are Parts depicted as Lifelines (notation: rectangle with a dashed vertical line below)
• Combined Fragment operators support recursive nesting and Turing Complete semantics (Alternative [alt], Optional [opt], Parallel [par], Loop [loop], etc.)

The purpose of Sequence diagrams is to specify dynamic system behaviors as message-passing collaborations among prototypical Blocks (Parts).

To learn more about Sequence Diagrams, follow the link to the summary lesson on seq
(https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/9_Sequence%20Diagrams.md)

## State Machine Diagram (stm)

 A State Machine diagram is a dynamic behavioral diagram that shows the sequences of States that an object or an interaction go through during its lifetime in response to Events (a.k.a. "Triggers"), which may result in side-effects (Actions.
The purpose of State Machine diagrams is to specify dynamic system behaviors for time-critical, mission-critical, safety-critical, or financially-critical objects#.

To learn more about State,acjome Diagrams, follow the link to the summary lesson on stm
(https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/10_State%20Machine%20Diagrams.md)

## Use Case Diagram (uc)

 A Use Case diagram shows communications among system transactions (Use Cases) and external users (Actors) in the context of a system boundary (Subject; notation: rectangle). Actors may represent wetware (persons, organizations, facilities), software systems, or hardware systems. Defining relationships between the system Subject and the system Actors is an effective informal way to define system scope.
The purpose of Use Case diagrams is to provide a high-level view of the subject system and convey the top-level system requirements in non-technical terms for all stakeholders, including customers and project managers as well as architects and engineers.

To learn more about Use Case Diagrams, follow the link to the summary lesson on Use Cases
(https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/3_Use%20Case%20Diagrams.md)
