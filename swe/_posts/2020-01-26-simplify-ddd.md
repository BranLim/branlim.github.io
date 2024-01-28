---
title: "Agile Software Development Process - Simplifying Domain Driven Design" 
permalink: /swe/:title
collection: swe
category: swe
date: 26 January 2020
excerpt: An article on simplify Domain Driven Design
---

There are many software development approaches that have been thought up and practised by software engineers around the world.

Domain Driven Design (DDD) is one such approach that was introduced and popularised by Eric Evans in the blue book of the same name that was published in 2004. It uses and expands on the principles and concepts defined in Object Oriented Analysis and Design (OOAD). And, it is considered to be a type of agile software development process because it focuses on connecting the implementation to an evolving model.

Anyone who has picked up and read the Domain Driven Design book would know that it can be a heavy read and is mostly theoretical, making it very hard for people to get started on applying the concepts.

For this article, we will attempt to make DDD easy to understand and applicable to developers.

## What does domain mean in Domain Driven Design?

If you pick up a dictionary and look up the word, domain, you will come across an explanation that goes like this:

> A specified sphere of activity or knowledge.

But it still does not help us answer the question: what does this mean in the context of software engineering?

It refers to the subject area on which the software is intended to be used. For developers, you can think of it as the business logic of an application or the rules that define how each object in the system are related to and interact with each other to create and modify modelled data.

## What is Domain Driven Design?

In the context of Domain Driven Design, and continuing from where we left off before, Domain Driven Design is basically an approach to software development where the "business logic" of an application is the king of the hill; not the RESTful APIs that other applications need to interface with or the databases needed to store the data. The business logic is modelled out in the form of complex objects, properties and behaviours.

But that is not all of it.

Domain Driven Design is also about the software team collaborating with domain experts or subject-matter experts to improve the application model and resolve any domain-related issues.

There are also several terminologies introduced in Domain Driven Design book by Eric Evans that are useful when describing and discussing DDD practices:

- **Context**\
  It refers to the setting in which a word or a statement appears that determines its meaning. For example, the word 'flight' can take on different meaning depending on when and where it is used even within the airline industry.

- **Model**\
  The domain model is a representation of the concepts and their relationships in a given domain. As a system of abstractions, it describes selected aspects of the domain and can be used to solve problems within it.

- **Bounded Context**\
  A bounded context is logical boundary within which a particular model is defined and applicable. We can think of the bounded context in the same way as each nation within the Associations of Southeast Asian Nations (ASEAN) or the European Union (EU) having its own official language and policies that do not necessarily apply to its neighbours.

- **Ubiquitous Language**\
  It refers to the language structured around the domain model that simplifies and standardises the vocabulary used. The software team can used it to connect their activities with the software.


### Building blocks of Domain Driven Design

We cannot implement Domain Driven Design without first understanding and knowing about the high-level concepts that were defined for the purpose of creating and modifying the domain model. In other words, there are tools that are specific for solving a particular issue within the domain.

- **Entity**\
  An entity is an object that is identified by its consistent thread of continuity and has a unique identifier (e.g. A person or user).
- **Value Object**\
  An immutable object that has attributes but no identity. (e.g. Money or Currency)
- **Domain Event**\
  An object that is used to record discrete event related to model activity within the system.
- **Aggregate Root**\
  An aggregate root is a type of entity that group a cluster of entities and value objects within a given bounded context. It serves as the main entry point from which external objects and client codes will access and/or modify the various entities and value objects. Ideally, an aggregate root has its own matching repository.
- **Service**\
  Not to be confused with application service, a service is an operation or a form of business logic that does not naturally fit within the realm of an object.
- **Repositories**\
  In DDD, a repository is a service that uses a global interface to provide access to entities and value objects that are within an aggregate collection. It should come with methods that allow for creation, modification, deletion of objects within the aggregate.
- **Factories**\
  Factories encapsulate the logic of creating complex objects and aggregate, which ensure the client has no knowledge of the inner-working of object manipulation.


### Advantages of Domain Driven Design

**Better User Experience**

When the whole software team utilises domain driven design, domain terms can be captured at the code level such as during the naming of the software classes and their methods. Furthermore, the team could also ensure the software frontend is a reflection of the domain model by using the same terms from the ubiquitous language and implementing the same behaviours described by the APIs. This way, the users of the software have a better and easier time using it to achieve their goals.

**Improves Flexibility**

DDD is heavily based on OOAD concepts. Domain models will mostly be objects, which make them highly modular and encapsulated. This means that the domain models can be changed and improved upon much more easily throughout the software lifecycle.

**Ease of Communication**

Domain driven design emphasises on the early development of a common and ubiquitous language related to the domain model. This reduces the need for jargons, which can help make communication between domain experts and the developers easier and also minimises confusion.

### Disadvantages of Domain Driven Design

**Requires robust domain expertise**

It is not enough for a software project to have a team of technically proficient people working on it. If these people do not know the intimate details of the subject area on which the application will be used, there is a high chance the final product will fail to meet the business requirements. The project team would need to collaborate with domain experts or have team members who can act as the subject matter experts during the development lifecycle.

**Encourage iterative practices**

In a software project, being able to do iterative development is an advantage because requirements change all the time. However, it is a disadvantage for organisations that have been doing software projects using the waterfall methods and are unable to change their processes due to resource or talent limitation.

**Not suitable for highly-technical project**

DDD places a heavy emphasis on the importance of having domain experts to create proper ubiquitous language and domain models for the project. This makes it useful for situations where the business logic is extremely complex and convoluted.

However, it is not suitable for projects that are technically complex but have marginal complexity in terms of business logic. For such projects, the domain experts may not be able to contribute effectively since they might not be able to grasp the problem.


 

