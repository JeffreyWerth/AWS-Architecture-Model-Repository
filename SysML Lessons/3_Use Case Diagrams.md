# Use Cases

Use Cases provide means for describing basic functionality in terms of usages/goals of the system by actors.

*Lesson 3 reading: SysML Distilled - A Brief Guide to the Systems Modeling Language 1st Edition Chapter 5 Use Case Diagrams*

## Use Case Basics

Use Cases are externally visible services a system provides, depicted in an ellipse, as a verb or phrase. The Use Case specification conveys the narrative that unfolds when a primary actor invokes the use case.

What does a use case diagram conveys?
- A set of use cases and actors that invoke and participate in them
- Invoke (primary); participate (secondary)

Use Cases is a classifier, an element of definition, please reference Lesson 4_Elements of Definition vs Usage to better understand this concept.

## Use Case Diagram Components

Use Case Diagrams are comprised of the following:
- Subject
- Actors
- Use cases
- Relationships

See Example Figure 5 bellow.

![Use Case Example](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/AWS%20Use%20Case%20Lesson%20-%20Use%20Case%20Example.svg)

<https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html>
<https://docs.aws.amazon.com/AmazonS3/latest/userguide/monitoring-automated-manual.html>
### Subject

Subject provides functionality in support of the use cases, represents a system being developed, also called the 'system under consideration', in this case the AWS S3 Service. The subject is represented by a rectangle on the use case diagram, see Figure 6.

![Use Cases Subject](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/AWS%20Use%20Case%20Lesson%20-%20Use%20Case%20Subject.svg)

### Actors

Actors used to represent something that uses the system, but not 'part' of the System, simply actors interface with the system. 

Actors can be a person or another system, usually depicted by a stick figure and/or block with **<<<actor>>>** label, see Figure 7. Name the Actors base on the **role** they perform as a user of the system (e.g. customer, administrator, developer etc).


![Use Case Actors](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/AWS%20Use%20Case%20Lesson%20-%20Use%20Case%20Actors.svg)
### Use Cases or Actions

Actions are represent the goals that a system will support, depicted by an oval with the Use Case name inside. Name should consist of a verb and a noun that descirbe the functionality of the system (e.g. Deploy Static Website, Deploy Website, Log Web Traffic and Create a bucket)

![Use Cases Actions](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/AWS%20Use%20Case%20Lesson%20-%20Use%20Case%20Actions.svg)
### Relationships

- Include - depicts shared (or re-used) functionality
- Extend - depicts optional functionality, performed when a particular condition is met
- Classification - indicates that the specialized Use Case inherits functionality from the general Use Case

![Use Cases Relationships](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/SysML%20Lessons/Lesson%20Views%20and%20SVGs/AWS%20Use%20Case%20Lesson%20-%20Use%20Case%20Relationships.svg)

## Summary
 - Use Cases capture the functionality a system must provide to achieve user goals
 - Use Case diagrams are made up of:
    - Subject
    - Actors
    - Use Cases or Actions
    - Relationships
- Use Case can be elaborated through:
    - Activity Diagrams (Lesson 8)
    - Sequence Diagrams (Lesson 9)
    - State Machine Diagrams (Lesson 10)
