# A UML Profile for Domain-driven Design of Microservice Architectures

This repository contains an early version of a UML profile aiming at enabling the Domain-driven Design (DDD) of Microservice architectures. The profile has been implemented on the basis of Eclipse Papyrus as it is contained in the Eclipse Modeling Tools Neon.3 Release (4.6.3).

The profile currently defines stereotypes and constraints for the following DDD patterns:
  * Classes
    * AggregatePart and AggregateRoot
    * Entity
    * Repository
    * Service
    * Spec
    * ValueObject
  * Operation
    * Closure
    * DefinesIdentity
    * SideEffectFree
    * ValidatesSpec
  * Package
    * BoundedContext
    * Module
  * Property
    * DefinesIdentity

The profile is contained in the file "ddmm.profile.uml". To use the profile, follow these steps:
  1. Create a new Eclipse Papyrus project with Diagram Kind "Class Diagram" (preferably with the Eclipse Modeling Tools).
  2. Copy the file "ddmm.profile.uml" into the project.
  3. Apply the profile on the diagram created in Step 1.
  4. Model your class diagram and apply DDD stereotypes as necessary.
  5. Right click on your class diagram and choose "Validation --> Validate model" to perform validation of the OCL constraints embedded in the profile.

Additionally, the repository contains a profile-based, valid Papyrus model "testmodel.uml" partially taken from [1].

For a comprehensive and more formal introduction of the profile, please refer to the preprint of our paper for the Workshop on Microservices: Science and Engineering (MSE) at https://mse-sefm17.fbk.eu/papers/paperMSE1.pdf.


### References
1. Evans, E.: Domain-Driven Design. Addison-Wesley (2004)
