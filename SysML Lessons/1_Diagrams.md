# Systems Modeling Language (SysML)

The Object Management Group Systems Modeling Language (OMG SysML), simply stated as SysML, is a general-purpose modeling language for systems engineering applications.

SysML supports the specification, analysis, design, verification, and validation of a broad range of systems. SysML consists of Abstract Syntax and Concrete Syntax:
- Abstract Syntax is the set of rules that identify what you can and cannot do
- Concrete Syntax is the set of notations that you are allowed to use on diagrams

## What are SysML Diagrams?

- Diagrams are elements in your model
- Diagrams are views of the model
- The model itself is generally shown as elements within a hierarchical structure of nested packages (often referenced as the CSM term: Containment Tree)
- A diagram is a partial graphical representation of the model that is generated to satisfy a stakeholder’s request
- A diagram can also be a partial graphical representation of the model element that the diagram represents
- An item can exist in your model without being shown on any diagrams
- A set of diagrams does not need to completely cover the model
- Deleting an item from a diagram does not remove it from the model
- Deleting a diagram does not affect the elements, or the relationships between elements, that were displayed on that diagram

## Diagrams Format

![Diagram Format](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/SVGs/Diagrams%20Format.svg)


### Header Format - diagramKind

SysML-defined acronym identifying the kind of diagram shown:
- activity diagram (act)
- block definition diagram (bdd)
- internal block diagram (ibd)
- package diagram (pkg)
- parametric diagram (par)
- requirement diagram (req)
- sequence diagram (sd)
- state machine diagram (stm)
- use case diagram (uc)

### Header Format - [modelElementType]

Remember that diagrams are model elements and they have a name and a type.
modelElementType is determined by the element that the diagram represents.

The most common element types per diagram kind are as follows:

- act: activity
- bdd: block, constraintBlock, package, model, modelLibrary, view
- ibd: block
- pkg: package, model, modelLibrary, view, profile
- par: block, constraintBlock
- req: package, model, modelLibrary, view, requirement
- sd: interaction
- stm: stateMachine
- uc: package, model, modelLibrary, view
### Header Format - modelElementName

Remember that diagrams are model elements and they have a name and a type. modelElementName is the name of the model element that the diagram represents

### Header Format - [diagramName]

This can be anything you would like, but should be a brief name to provide the reader some knowledge on what they should expect to see in that diagram.
