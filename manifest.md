# Wright Manifest

## Core Schema Structure

* Metadata: Global identifiers, versioning, and the target analysis layer (Container, Component, or Code).
* Entities (Nodes): The structural building blocks representing the actual architecture (e.g., Services, Repositories, Classes, Interfaces).
* Relationships (Edges): The defined connections between entities (e.g., calls, implements, depends on).
* Constraints (Rules): The explicit architectural rules that Wright must enforce post-validation (e.g., isolated layers, forbidden dependencies)./We’re going to split the system architecture into 4 layers to show how users can use Wright.

### System Context

Not in the target.

### Containers

Composing only communications between applications. Reference metadata would be assigned to each application to indicate that this collection of code presents an application.

### Components

Search semantically for active components, connections, and communication protocols established in the code.

### Code

Compare the UML diagrams with the actual code. Parse the code and compare it with the semantics of the design. Could have a project structure document to make it easy for parsers to find classes and features.

## What is the unified format to be used as input?

We intend to follow the C4 model with UML structure to illustrate internal components, classes, and flows. Most of the elements are custom and have post-validation functionality to be described in the parsing process (For example, an interface block holds the engineering definition of an interface so the corresponding code is judged based on an interface behaviour).
