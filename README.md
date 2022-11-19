# AWS-SysML-Architecture-Model-Repository

The AWS SysML Architecture Model Repository, is an open source project on GitHub for any Systems Engineering professionals or students to collaborate and learn how to model cloud systems using SysML.

## Objectives

At the end of this independent project, the student should have an awareness of:

- model-based systems engineering approach
- SysML language and modeling abstract systems
- How SysML is use as part of an MBSE process.
## Scope

AWS as a cloud platform (<https://aws.amazon.com/marketplace/solutions/awsmp-all-use-cases>) has more than one hundred cloud services, which enable organizations to secure, store and compute their data on the cloud. This benefits the organization in a way that there is no need for physical hardware to manage the IT infrastructure of the organization.

The intent of this open source project on GitHub, is to model these services using SysML to better understand how these services impact the enterprise, and help organizations transferring their data from physical applications to cloud-based infrastructure, applications, and legacy systems; with the goal to understand any security impacts on how the data is manage and transfer using SysML to model the interfaces that makes these IT systems live in the Cloud.

Attached in this repository, is an AWS SysML Architecture Model Dictionary and Glossary to catalog the model elements that will make a library of systems and services that makes the AWS ecosystem. The library of model view will remain as a project in GitHub, for the Systems Engineering community, to learn how to model Cloud Systems by Systems Modeling Language (SysML).

## Expected Results and Using Github

The independent project submission for any of the model elements chosen by the Systems Engineer, shall follow the requirements of OMG Systems Modeling Language version 1.6. The model views shall follow the following GitHub S3 Example under SysML Modeling Notes and Examples, with the intent to follow the OMG Standards when presenting the views of the system under consideration. When starting a new project recommend forking this repository and restructuring to follow the file structure and then deleting everything in the README section up to the SysML Modeling Notes and Examples to submit your project.

The submission shall have the following sections:

- Model Description and Dictionary
- Structure Diagram Views
- Behavioral Diagram Views
- Requirements Diagram Views

### Point of Contacts

If you need help setting up and getting started with your project. Please use the following information to get a hold of me.

Michael L Kent
kentmichae@gmail.com
michael.kent@gdit.com

## Modeling and SysML Standards

SysMl is simple but powerful graphical constructs for modeling a wide range of systems engineering problems. Is perfect in addressing system complexity by specifying requirements, structure, behavior, allocations, and constraints on system properties to support engineering analysis/system tradeoffs.

SysML reuses a subset of UML 2 and provides additional extensions to satisfy the requirements of the language. For the project, we are referencing OMG SysML version 1.6 cited in the Primary Standards Section. I also recommend reading SysML Distilled: A Brief Guide to the Systems Modeling Language 1st Edition by Delligatti and following the OMG Systems Modeling Language
(OMG SysML™) Tutorial from September 2009 in the additional references section.

### SysML Diagrams

![SysML Diagrams](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/Views/SysML_Diagrams.svg)

### Primary Standards

OMG SysML available specification (formal/2007-09-01)
<https://www.omg.org/spec/SysML/1.6/Beta1/PDF>

### Additional References

SysML Distilled: A Brief Guide to the Systems Modeling Language 1st Edition
OMG Systems Modeling Language (OMG SysML™) Tutorial from September 2009 by Sanford Friedenthal/Alan MooreRick/Steiner

## AWS Model Repository Packages

The repository will be organize using the following packages ..............

## Software and Open Source Tools

This open source project in GitHub will utilize open source tools to create the SysML views, and manage the content of your model through VSCode. Also I recommend you get a free Github account for this project so you can clone and utilize most of the formatting and section contents when creating views of your model.

To install drawio-desktop use the following GitHub repository (<https://github.com/jgraph/drawio-desktop/releases>) where you can download and install the diagraming tool to create views of your model. As you can find in the Packages folder , there is already a folder for the S3 diagrams and views of the diagrams generated from the AWS S3 Service.drwawio file.

VSCode is a code editor redefined and optimized for building modem web and cloud applications and to manage your project using markdown language; this will allow you to fork this project and to rapidly create your model views (<https://code.visualstudio.com/>).

Also join Github (<https://github.com/>) to create and account so you can for the main project, and when publishing your project to GitHub for evaluation you can submit your model views. There is some good resources on how to clone
### SysML Modeling Notes and Examples

#### AWS S3 Service [Model Description and Dictionary]

Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can use Amazon S3 to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides management features so that you can optimize, organize, and configure access to your data to meet your specific business, organizational, and compliance requirements.

| Acronym   | Appointment | Description | Source | Model Element | Notes |
| --------- | ----------- | ----------- | ------ | ------------- | ----- |
| Header    | Title       |             |        |               |       |
| Paragraph | Text        |             |        |               |       |

#### AWS S3 Service [Structure Diagrams]

##### AWS S3 Service Bucket bdd

![AWS S3 Service Bucket](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/Packages/S3/AWS%20S3%20Service-S3%20Bucket%20bdd.svg)

##### S3 Service Storage Classes bdd

![AWS S3 Service Storage Classes](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/Packages/S3/AWS%20S3%20Service-S3%20Storage%20Classes%20bdd.svg)

#### S3 Service [Behavioral Diagrams]

##### S3 Service Lifecycle Classes stm

![AWS S3 Service Lifecycle](https://github.com/kentmichae/AWS-Architecture-Model-Repository/blob/main/Packages/S3/AWS%20S3%20Service-S3%20Lifecycle%20stm.svg)

#### S3 Service [Requirements Diagrams]
