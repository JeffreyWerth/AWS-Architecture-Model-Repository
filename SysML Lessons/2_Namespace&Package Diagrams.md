# Namespace and Package Diagrams

This section will go over the concept of Namespace and Package Diagrams.

*Lesson 2 reading: SysML Distilled - A Brief Guide to the Systems Modeling Language 1st Edition Section 2.4 and Chapter 10 Package Diagrams*

## Namespace

Otherwise known as ‘where is something contained in the model’. A diagram’s modelElementName and modelElementType identify the default namespace for the elements shown on that diagram.

A qualified name for a model element is required anytime the element shown on a diagram that is not contained within the default namespace, Why? to properly define the location of that element within the model.

## Packages

The Packages also represent a namespace for the contained model element a unique name within the model. Packages are both containers and namespaces.

SysML models are organized into a hierarchical tree of packages that are much like folders in a GitHub repository structure. Packages will be used to partition elements of the model into directories that can be subject to manage content of the repository.

### Package Diagram for AWS SysML Architecture Repository


## Package Diagram Containment Relationship