# Namespace and Package Diagrams

This section will go over the concept of Namespace and Package Diagrams.

*Lesson 2 reading: SysML Distilled - A Brief Guide to the Systems Modeling Language 1st Edition Section 2.4 and Chapter 10 Package Diagrams*

## Namespace

Otherwise known as ‘where is something contained in the model’. A diagram’s modelElementName and modelElementType identify the default namespace for the elements shown on that diagram.

A qualified name for a model element is required anytime the element shown on a diagram that is not contained within the default namespace, Why? to properly define the location of that element within the model.

## Packages

The Packages also represent a namespace for the contained model element a unique name within the model. Packages are both containers and namespaces.

SysML models are organized into a hierarchical tree of packages that are much like folders in a GitHub repository structure. Packages will be used to partition elements of the model into directories that can be subject to manage content of the repository.

The diagram kind abbreviation for a package diagram is pkg. The model element type that the diagram frame represents can be any of the following:
- package
- model
- modelLibrary
- view
- profile

To further learn about the specialized packages read Section 10.7 from *SysML Distilled - A Brief Guide to the Systems Modeling Language 1st Edition*.

### Package Diagram for AWS SysML Architecture Repository

The AWS SysML Architecture Repository is organized by AWS Services and Use Cases, bellow is Figure 3 AWS Package Diagram Example.

![AWS Package Diagram Example](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/AWS%20Package%20Diagram%20Lesson.svg)

A **model** is one of four specialized kinds of packages; it's the kind of package that serves as the root of a containment hierarchy.

## Package Diagram Containment Relationship

The Figure 4 bellow uses two type of containment relationships, first the crosshair notation appears as a solid line with a circled plus sign on the namespace end of the relationship and second the next notation for namespace containment is the nesting notation. The notation is used in Figure 4 to convey that the Analytics package contains the three analytics services: Amazon Redshift, Amazon QuickSight and Amazon Athena.

![Package Diagram Containment Relationship](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/AWS%20Package%20Diagram%20Lesson%20-%20Containment%20Relationships.svg)

### Dependencies between Packages

Figure 4 shows seven dependencies-the dashed lines with open arrowheads-drawn between packages. The package diagram in FIgure 4 conveys that a change to the contents of any of the seven service packages may result in a change to the contents of the Use Cases package.