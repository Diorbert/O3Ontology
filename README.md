![](logo/logo.png)

# Authors

* Diorbert Pereira
* João Paulo Andrade de Almeida

# The O3 Ontology

The industry’s need for enterprise architecture description has been supported by many approaches that include ontologies and languages. Despite the alternative solutions, some approaches have specific purpose and shortcomings with consequences in precision and coverage. The OntoUML Organizational Ontology (O3) is a well-founded core ontology, built with the purpose of serving as a reference ontology for organizational definition. It is intended to support the creation of domain ontologies through the specialization of its concepts and relationships, as well as to support the analysis and revision of EA languages. 

* [Reference Model](doc/reference_model.md)
* [Organizational Structure View](doc/organizational_structure_view.md)
* [Organizational Roles View](doc/organizational_roles_view.md)

## Organizational Roles View

The organizational role view describes the roles that specify the expected behavior of the organizational members. As a consequence of the independent nature of organizations, the individuals (natural persons) that compose an organization can change over time. The defined set of roles has the purpose of keeping the organization on course of their goals while maintaining the uniformity of the expected behavior of its members. These roles are called social roles and are defined by normative descriptions. The establishment of social roles by a recognized authority is fundamental, once only the recognition of its act assigns validity to the characteristics inherent to the role. Figure 47 presents the social role hierarchy.

Figura 47

The main concept, business social role, describes a role defined and valid on the scope of an organization. It is refined in business role, employee type and collaboration business role. The complete specialization hierarchy of business social roles encompasses the roles presented in Figure 47. Here, we will not go into more detail about the taxonomy of business roles, as these concepts will be defined in later sections.

In an organizational structure description, it is important to define the relationship between the behaviors of the individuals with the collective behavior. In this context, we can describe the behavior of an organizational units by the specification of a set of business roles (through the “inherent to” relationship). For example, it’s very natural to say that the Sales Department is associated with the Salesman and the Sales Manager roles. This association does not bind the people with an organizational unit, but specify the behavior that the members of it have to assume. Figure 48 presents the recognition chain between organizations and their members, normative descriptions and social roles. The fragment presented in Figure 48 comprises an upper vision about “recognition” relationships, which are extended to create specific relationships to the active structure domain. 

Figura 48

In organizational scope, we have a special type of social role, namely business social roles, which are formalized by internal regiments. An internal regiment is a specific type of normative description and has its scope limited to the organization. Formal organizations define internal regiments to describe formally their roles, which are recognized by their organizational units and members. 

In an upper view of the “recognition” subject, we have normative descriptions as a central part. A normative description, as defined in (GUIZZARDI; FALBO; GUIZZARDI, 2008), defines one or more rules/norms recognized by at least one social agent. We extend here the notion of recognition defining social entity. The essence of organizations is social, but, as a social agent, an organization is composed by natural persons. Within the organization, a natural person assumes a social role against the whole, becoming a social entity. The difference between organizations and organizational members as social entities lies in the fact that an organization always will be a social entity, while an organizational member may cease their role in the organization. At this level of analysis, normative descriptions may be defined by organizations. In a lower view, the “defines” relationship between formal organization and internal regiment is “redefined”. At this configuration only formal organization are entities with the right of defining normative descriptions. Figure 49 extends the concept of recognition illustrating the discussion about recognition contracts.

Figura 49

Like living organisms, organizations adapt to changes in their external environment. Organizational evolution generally comes with changes in organizational structure (departments and roles). The maintenance of the formal environment is coupled with continuity of the formal recognition by the individual and collective agents against the organizational definitions. Here, we call definition every role defined, every organizational unit create. With this in mind, a recognition contract describes a formal agreement between social entities. On one side, a social entity creates (generates) the recognition contract and its attachments (maybe at a later time). On the other side, the recognition contract and attachments are accepted and consequently the normative descriptions associated with the contract also are recognized. 

Normative descriptions can be related with many recognition contract (and its attachments). In contrast, a specific recognition contract may be related with one or more normative descriptions. 

To visualize this recognition arrangement, take the following example. A software development company decided to terminate the “mathematical models department”. For this, the organization has created new positions to meet the functional need and relocated former members of the “mathematical models department” to other departments. For such changes to be valid, it is necessary that all members of the organization recognize its legitimacy. We can observe this scenario as an update of an existing recognition contract. In this case, a recognition contract attachment is associated with the normative description that formalizes the creation of the new position. The “accepts” relationship between the social entity and the recognition contract attachment is derived by the specification of the relationship of “attachment of” between the recognition contract attachment and the recognition contract. Note that we not intent to enter in legal matter about additional agreements on updating an existing agreement. Our purpose here is to describe the continuous formal characteristic of organizational acts.

Table 9 presents the constraints that must be observed on analyzing or instantiating of the concepts of the Organizational Role View.

|ID | Description |
|----------|-----------------------|
|AXI10|	A “Social Entity” that defines a “Normative Description” should compulsorily recognize it.|
|AXI11|	If an “Organization” recognizes a “Normative Description”, automatically its members should also recognize it.|
|AXI12|	A “Structural Business Role” inherent to a “Structural Unit” will result in a definition relationship between the organization as a whole and the business role.|
|AXI13|	A “Missionary Business Role” inherent to a “Missionary Unit” will result in a definition relationship between the organization as a whole and the business role.|
|AXI14|	If a social entity accepts (recognizes) a Recognition Contract then this entity must also recognize the Normative Descriptions associated with this contract.|

## Allocation View

The allocation view describes the establishment of the relation between the members of the organization and the organization itself, including its sub-organizations. Figure 50 presents the most basic arrangement for the definition of a member of the organization. Here, we are only concerned with human agents, and thus the physical agents we refer to are human beings, i.e., natural persons. The association of natural persons to an organization is an essential part of the definition of organizations, being defined by an organizational membership. By becoming an organizational member, a natural person is inserted among a group of agents that comprise the organization. An organizational member is the most generic denomination of a member of the organization is refined in more specific types of members, according to the allocation type (admission or assignment). 

Figura 50

In the scope of each organization, different specializations of these more general roles are required. For example, in a university, employee types such as “University Professor” and “Secretary” become relevant, while in a hospital employee types such as “Doctor” and “Nurse” may be defined. Therefore O3 includes the second-order notions of employee type and other business roles. They are to be instantiated in particular settings creating thus specific roles. The instances of employee type extend formal organization member, and the instances of business role extend either structural unit member or missionary unit member. We represent them by following the UML’s “powertype” representation pattern with the second-order concept stereotyped <<hou>> (for higher order universal), highlighted in gray. Due to this, the user of the ontology can develop an extension that includes specific roles to his/her domain of interest. Figure 51 illustrates this setting.
  
Figura 51

Figure 52 and Figure 53 present in details the concepts related with the agents that compose the organization and the types of roles they may play. In these fragments, we are concerned with the specific roles that natural persons play, first of all as a member of a formal organization (Formal Organization Member), and then when they are given more specific places in the power structure, either in a structural (line or staff) unit (Structural Unit Member) or in missionary units (Missionary Unit Member). Note that in order to play a particular role in an organizational unit, a person needs to be a formal organization member first. Figure 52 defines in detail the existing formal relation between an employee and a formal organization.

Figura 52

The association between an individual and an organization is accomplished through an admission or an assignment. When an individual becomes an employee (Formal Organization Member) of an organization, her formal “link” with the employer is the action of admission. The admission defines, in a general way, the expected behavior and constraints through the association of the individual with an employee type. In addition, an admission is recognized by the external environment, e.g., a real estate recognizes that Paul is a mechanical engineer (his profession) in a lease process.

Specific employee types define the set of roles (business roles) that a typified employee can occupy in the organization (through the “cover” relationship). Business roles define more specific capabilities, duties and prerogatives possibly in the scope of organizational units. Thus, business roles are more committed with the expected behavior than employee types once aggregate functional responsibilities (see Figure 56 for detail about functional responsibility). 

Formal organization members assigned to business roles are named performer member. In this scope, the allocation is limited to only the definition of functional responsibilities and does not extend to the allocation in organizational units. This setting fits perfectly with organizations that are not constituted by organizational units (simple standalone functional/missionary organizations). Figure 53 defines in detail the existing relation between an employee and organizational units.

Figura 53

Within the organization, an employee must be assigned to an organizational unit to assume a specific role and consequently a specific function. An assignment is recognized only in the internal context of the organization and can be structural (structural assignment) or missionary (missionary assignment). When an assignment is related with the allocation of an employee to a structural unit, the individual becomes a structural unit member, whose subclasses are instances of structural business role. An employee allocated to a structural unit must play a structural business role; on the other hand, employees assigned to missionary units play missionary business roles. This type of assignment represents for example the association of John to the role of “system analyst” in the “IT department”.
Organizations that adopt the matrix structure can perform multiple assignments of “functions” to their employees. Generally, an employee is allocated to only one structural unit, but it is possible that the same employee is assigned to different missionary units, with different missionary business roles. When associated to a missionary unit, an employee becomes a missionary unit member. The specializations of the concept missionary unit member are instances of missionary business role.

When assigned to an organizational unit, an employee has a defined “function” formalized in the specification of the business role, which defines in detail its expected behavior and authority relationships. The accumulation of “functions” by an employee can be simultaneous or at different time periods. The assignments are only possible if the individual is member of the organization, not being possible, for example, that John is allocated (by an assignment) to an organizational unit if he is not a member of the organization or a member of another organization. Thus, the assignments are tied with the admission that made the individual a member of the organization, which is defined through the relationship “refers to”. 

Admissions and assignments can be performed through many actions (e.g., an election, an appointment), each of these defining a different member. Figure 54 describe in detail the multiple membership forms. 

Figura 54

Before discussing the many forms of membership (admission and assignment), we need first to define election and appointment. An election is a process to select one among many candidates. In an election many electors participate with votes to a specific candidate. The candidate with the most votes is selected. In contrast, an appointment is performed by a nominator in favor of other. 

In the organizational context, an employee may be admitted or assigned by different forms. An effective membership is the most common admission/assignment type and represents an admission/assignment following the usual process. Other forms of membership include appointments and elections. When an employee is admitted as consequence of an appointment, the resulted admission/assignment is a membership by appointment. An appointment need not necessarily be performed by members of the organization. In the case of O3, a natural person or a social agent can “realizes” an appointment. Finally, an employee can be elected by a group of natural person or social agents, which “participates” of its selection. The presence of social agents in appointment process can be observed, for example, United Nations Council. The General Secretary is appointed by the General Assembly, after being recommended by the Security Council. The members of General Assembly are governments, which represents social agents.

Table 10 presents the constraints that must be observed on analyzing or instantiating the concepts of the Allocation View.

|ID | Description |
|----------|-----------------------|
|AXI15|	Every member of an organizational unit should be employee (Formal Organization Member) of the “Formal Organization” to which the “Organizational Unit” is related (component of relationship).|
|AXI16|	An employee (Formal Organization Member) can only assume a “Business Role” inherent to the “Organizational Unit” to which he/she belongs.|
|AXI17|	An instance of "Business Role" cannot establish a relationship "covers" with itself.|
|AXI18|	Assignments should be performed in the context of a specific “Admission” in an organization (Formal Organization), i.e., an instance of "Formal Organization Member", which was admitted by an admission a1, cannot have a related assignment with an admission a2.|

## Social Relationships View

The social relationships view describes how the members of an organization are related. During the length of stay of an employee in an organization, he/she plays many roles that are internal to the same. These roles formalize the social contract between the employee and the organization, defining the expected behavior and social relationships, like authority and communication. Figure 55 presents the social relationships that permeate organization members.

Figura 55

As a coordinated environment, authority constitutes a fundamental aspect for organizations. Authority is related with the formal assignment of power to an employee with respect to another. In terms of O3, a formal organization member “is superior to” another. Despite the fact of the “is superior to” relationship be used in many ways between structural business roles and missionary business roles, its meaning varies in according to each use. The reflective authority relationship “is superior to” that occurs between structural business roles and missionary business roles allows the differentiation between the command structure of a department and the command structure of a project, for example. In addition, in many organizations those responsible for projects, task forces and others, are not allocated in the associated missionary unit, but participate giving the directives, constraints and demanding results to the leader of the working group. The power relationship existing between structural business roles and missionary business roles also can be defined through the “is superior to” relationship. 

The establishment of power relationships provides managers a way to achieve the coordination of the actions to fulfill goals. To support horizontalization, cooperation must also be present in social structure. Cross functional processes are performed by multidisciplinary participants in a cooperative way. Cooperation allows the interaction between the participants without the establishment of authority, describing that a member “relates with” another. This relationship also can be viewed as a communication link between the participants.

In some cases, the rigid authority structure is not adequate for agile decision making. Usually, managers delegate part of their authority in favor of breaking down decision barriers. The authority delegation allows empowerment of a performer member to a specific duty (functional responsibility). E.g., a sales manager may delegate authority to a salesman to ensure that a particular sales process is followed. While the delegation is not revoked the salesman has authority over the staff related with the functional responsibility. Figure 56 illustrates organizational delegations, regarding of authority and functional responsibility.

Figura 56

The goals pursued by an organization can be decomposed at its lowest level of decomposition into tasks (DO; FAULKNER; KOLP, 2003). The distribution of tasks is performed by the assignment of functional responsibilities to its members as duties (delegation). Performer members may have multiple functional responsibilities, carried out in the context of their business roles. Functional responsibilities aggregate many functional commitments. The difference between functional responsibilities and commitments lies on the basic nature of these two concepts. The first represents the delegation of responsibilities to someone, while the last describes the tasks that must be performed. A functional commitment does not represent a specific task, but instead a predisposition to conduct tasks. We choose to not describe the activities related with a specific functional commitment, since behavioral aspects are out of our scope. The user of the ontology can alternatively integrate or extend the ontology to cover behavioral aspects. For this, we recommend the use of the functional commitment concept as a bridge.

Table 11 presents the constraints that must be observed on analyzing or instantiating the concepts of the Social Relationships View.

|ID | Description |
|----------|-----------------------|
|AXI19|	A structural role (Structural Business Role) may be superior to structural roles defined by the same organization (Formal Organization) to which it belongs.|
|AXI20|	A team role (Missionary Business Role) can only be superior to team roles defined by the same organization (Formal Organization) to which it belongs.|
|AXI21|	A structural role (Structural Business Role) can only be superior to team roles (Missionary Business Role) defined by the same organization (Formal Organization) to which it belongs.|
|AXI22|	An instance of "Structural Business Role" cannot establish a relationship "is superior to" with itself.|
|AXI23|	An instance of "Missionary Business Role" cannot establish a relationship "is superior to" with itself.|
|AXI24|	An instance of "Structural Unit Member" cannot establish a relationship "relates with" with itself.|
|AXI25|	An instance of “Structural Business Role” cannot establish a relationship “is superior to” with someone that is transitively superior to it.|
|AXI26|	An instance of “Missionary Business Role” cannot establish a relationship “is superior to” with someone that is transitively superior to it.|

## Business Collaboration View

The business collaboration view describes the external organizational interactions and their participants. Despite the effort to define organizations as a unit, the view that organizations are inserted in a broad collaborative and dependent environment is defended as the path to business survival. Organizations think of themselves as teams that create value jointly rather than as autonomous companies that are in competition with all others (DAFT, 2010). An organization interacts with suppliers to get its inputs, and, surely, interacts with its customers to sell its products or services. These interactions are called business collaborations. The knowledge about the context of the organizations is essential to business strategy, as a way to adapt the organizational behavior to the changes and opportunities (DAFT, 2010). Figure 57 presents the roles involved in business collaborations.

Figura 57

Business collaborations involve two distinct parts that work together to perform a collective behavior, an internal and an external part. Internal participants are namely internal collaborators and represent the organization as a whole (e.g., sales department, business agent). On the other hand, external participants are called external collaborators and represent the organizational environment (e.g., a supplier, a customer, an audit organization). Social agents or physical agents may get involved in a business collaboration. When an organizational unit (social agent) becomes an internal collaborator it plays the role of social agent internal collaborator. Similarly, when a formal organization member (physical agent) becomes an internal collaborator she plays the role of physical agent internal collaborator. 

An internal collaboration business role specifies the expected behavior of an internal agent when participating in a business collaboration. The specializations of both specializations of internal collaborator are instances of internal collaboration business role. This means that the specializations of both, social agent internal collaborator and physical agent internal collaborator, have as power type the internal collaboration business role concept. Due to this fact we can define types of roles explicitly in the model through specialization of these concepts, as shown in Figure 58.

Figura 58

Finally, when an organizational unit (social agent) becomes an external collaborator, it plays the role of social agent external collaborator. In the same way, when a natural person (physical agent) becomes an external collaborator, he/she plays the role of physical agent external collaborator. An external collaboration business role specifies the expected behavior of an external agent when participating in a business collaboration. The specializations of both specializations of external collaborator are instances of external collaboration business role. 

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
