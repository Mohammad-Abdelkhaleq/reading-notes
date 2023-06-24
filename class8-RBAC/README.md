### Code 401 - *Class 8 readings *

What is Role Based Access Control (RBAC) and why do we care?

*Role-Based Access Control (RBAC) is a security model that manages access to resources based on roles rather than individual users. It simplifies access management, provides granular control, enhances security, supports scalability, and aids in compliance and auditing.*

Describe a Role/Permission heirarchy that you might implement using RBAC.


*RBAC typically consists of roles arranged in a hierarchical structure, such as Administrator, Manager, User, and Guest. Each role is associated with a specific set of permissions, granting users access to the necessary functionalities and resources. The hierarchy ensures that higher-level roles inherit permissions from lower-level roles, providing a structured and controlled approach to access management.*

What approach might you take to implement RBAC?

* Identify roles based on job functions.

* Define specific permissions for each role.

* Assign roles to users based on their responsibilities.

* Establish a role hierarchy to determine inheritance of permissions.

* Implement access control mechanisms based on roles and permissions.
 
* Develop an interface for role and permission management.

* Regularly review and update the RBAC implementation to adapt to changing needs.

If Authentication is “you are who you say you are,” what is Authorization?

*Authorization is the process of determining and granting access rights to specific resources or functionalities based on the authenticated user's identity and assigned permissions. It decides what you are allowed to do or access after verifying your identity through authentication.*

Name three primary rules defined for RBAC.

1. **Role-User Assignment**: Users are assigned specific roles based on their job responsibilities and functions.

2. **Role-Permission Assignment**: Roles are associated with a set of permissions or access rights that determine the actions and resources a role can access.

3. **Constraint of Least Privilege**: Users are granted the minimum privileges necessary to perform their job functions, minimizing the risk of unauthorized access.

Describe RBAC to a non-technical friend.

*RBAC is a system that controls who can access what in an organization. It assigns different roles to people based on their responsibilities and allows them to access only the information and resources they need for their job. It helps maintain security, manage access easily, and ensures that people have the appropriate level of access.*











