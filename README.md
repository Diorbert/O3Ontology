![](logo/logo.png)

# Authors

* Diorbert Pereira
* João Paulo Andrade Almeida

# The O3 Ontology

The industry’s need for enterprise architecture description has been supported by many approaches that include ontologies and languages. Despite the alternative solutions, some approaches have specific purpose and shortcomings with consequences in precision and coverage. The OntoUML Organizational Ontology (O3) is a well-founded core ontology, built with the purpose of serving as a reference ontology for organizational definition. It is intended to support the creation of domain ontologies through the specialization of its concepts and relationships, as well as to support the analysis and revision of EA languages. 

* [Reference Model](doc/reference_model.md)
* [Organizational Structure View](doc/organizational_structure_view.md)
* [Organizational Roles View](doc/organizational_roles_view.md)
* [Allocation View](doc/allocation_view.md)
* [Social Relationships View](doc/social_relationships_view.md)
* [Business Collaboration View](doc/business_collaboration_view.md)

## Capability View

The capability view describes the organizational members’ characteristics relevant to performing their duties. Natural persons can be described by their physical and mental characteristics, like height, weight and temperament. These characteristics manifest themselves in the form of skills. In the organizational context, we are only interested in the subset of skills needed to carry out business tasks. Figure 59 presents the relationship between the required skills and the inherent skills of a natural person.

Figura 59

As defined in (FAYOL, 1949), each group of operations or functions corresponds to a special ability (skill). There are technical abilities, commercial abilities, financial abilities, administrative abilities, etc. The set of essential qualities and knowledge comprises physical, intellectual and moral qualities, general knowledge, experience and certain special knowledge regarding with a function to perform. This set of skills represent the requirements to engage in business social roles. In the scope of this work, we cover only physical and intellectual qualities, here called respectively, physical skill and cognitive skill. Examples of skills includes UML modeling, java programing, bridge structural design, flying aircraft, fast running and carrying heavy weights.

## Resource View

The resource view describes the organizational resources and their relationships with the organization and its members. Here, resources do not comprise human being as human resources, but only physical and social objects. A resource, in the sense of O3, follows rigorously the definition of resource in UFO-C. As defined in (GUIZZARDI; FALBO; GUIZZARDI, 2008), “only agents (entities capable of bearing intentional moments) can perform actions. An object participating in an action is termed a resource. Agents can be physical (e.g., a person) or social (e.g., an organization, a society). Objects can also be further categorized in physical objects and social objects. Physical objects include a book, a tree, a car; Social objects include money, language and Normative Descriptions”. In addition, we have also system objects, which represent software in general (e.g., an operational system, an ERP). A system object is not an agent, since we consider it cannot bear intentional moments, but have automated characteristics. Thus, this kind of objects participates as resources in actions. Figure 60 presents an overview of the definition of “resource” merging with UFO-C concepts. 

Figura 60

In the organizational scope, we also have particular objects, which can be possession of someone (owner) and are assigned to some organizational unit (available to the use). These objects are namely business physical objects. Many actions performed in the business context have the participation of resources. When a call center attendant makes a customer service, the description of the process is a social object, the phone used is a physical object and the software that records the occurrence is a system object. 

The access to a resource can be controlled by granting or revoking permissions. Group members (Figure 60) can maintain permissions over resources, as a permission provider or a permission holder. A permission holder can retain many permissions over many resources. On the other hand, as a permission provider, a group member can grant permission for many group members to access many resources. Note that the term “access” comprises use and consume.

Figure 61 presents the definition of organizational ownership and the roles involved.

Figura 61

An organizational ownership relates organizations with business objects as a possession relationship. The owner in an organizational ownership has certain rights with respect to the object. An ownership can be transferred by sale or donation (the transfer of ownership is out of the scope of our ontology). Despite the abstract nature of social objects, this kind of objects can be visualized as a property. Further, social objects also may have commercial value. An example of social objects owned by organizations includes the TOGAF Framework, Brazilian Real (currency) and ArchiMate modeling language. Despite the fact that system objects are abstract, a registered software has a transferable license which symbolizes the object itself.
