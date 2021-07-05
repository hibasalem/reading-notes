# Read: Class 8 : Access Control (ACL)

- - -

## Review, Research, and Discussion


* **When is Basic Authorization used vs. Bearer Authorization?**

basic Authorization login and Bearer Authorization to stay logeed in after log in 

* **What does the JSON Web Token package do?**

helps to authintacatet that some one is who he clames to be 

* **What considerations should we make when creating and storing a SECRET?**   

	* Never store unencrypted secrets in .git repositories. Avoid git add * commands on git. 		
	* Add sensitive files in .gitignore. Don't rely on code reviews to discover secrets. ...
	* Don't share your secrets unencrypted in messaging systems like slack.
	* Store secrets safely.
	* Restrict API access and permissions.

- - -

#### Document the following Vocabulary Terms

* **encryption** 

In cryptography, encryption is the process of encoding information. This process converts the original representation of the information, known as plaintext, into an alternative form known as ciphertext. Ideally, only authorized parties can decipher a ciphertext back to plaintext and access the original information.

* **token**    

a token is an object that represents something else, such as another object (either physical or virtual), or an abstract concept as, for example, a gift is sometimes referred to as a token of the giver's esteem for the recipient. In computers, there are a number of types of tokens

* **bearer**     

Bearer Tokens are the predominant type of access token used with OAuth 2.0. A Bearer Token is an opaque string, not intended to have any meaning to clients using it. Some servers will issue tokens that are a short string of hexadecimal characters, while others may use structured tokens such as JSON Web Tokens.

* **secret**    

JWT is created with a secret key and that secret key is private to you which means you will never reveal that to the public or inject inside the JWT token. When you receive a JWT from the client, you can verify that JWT with this that secret key stored on the server.

* **JSON Web Token**  
  
JSON Web Token is a proposed Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. The tokens are signed either using a private secret or a public/private key.

- - - 

## Preview

#### Introduction to JSON Web Tokens

* Which 3 things had you heard about previously and now have better clarity on?

	Tokens , jwt ,bearer authorization

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

	RBAC 

* What are you most excited about trying to implement or see how it works?
	 --

- - -

#### Role-based access control

In computer systems security, role-based access control (RBAC) or role-based security is an approach to restricting system access to authorized users. It is an approach to implement mandatory access control (MAC) or discretionary access control (DAC).

Role-based access control (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges. The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments. A study by NIST has demonstrated that RBAC addresses many needs of commercial and government organizations.RBAC can be used to facilitate administration of security in large organizations with hundreds of users and thousands of permissions. Although RBAC is different from MAC and DAC access control frameworks, it can enforce these policies without any complication.

#### Use and availability   

The use of RBAC to manage user privileges (computer permissions) within a single system or application is widely accepted as a best practice. A 2010 report prepared for NIST by the Research Triangle Institute analyzed the economic value of RBAC for enterprises, and estimated benefits per employee from reduced employee downtime, more efficient provisioning, and more efficient access control policy administration.
In an organization with a heterogeneous IT infrastructure and requirements that span dozens or hundreds of systems and applications, using RBAC to manage sufficient roles and assign adequate role memberships becomes extremely complex without hierarchical creation of roles and privilege assignments.Newer systems extend the older NIST RBAC model to address the limitations of RBAC for enterprise-wide deployments. The NIST model was adopted as a standard by INCITS as ANSI/INCITS 359-2004. A discussion of some of the design choices for the NIST model has also been published.

- - -

#### 5 steps to simple role-based access control (RBAC) 

RBAC is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.

* What is RBAC?

RBAC is nothing more than the idea of assigning system access to users based on their role within an organization. The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs. 

* Benefits of RBAC?

With the proper implementation of RBAC, the assignment of access rights becomes systematic and repeatable. Further, it is much easier to audit user rights, and to correct any issues identified.
RBAC may sound intimidating, but it can in reality be easy to implement, and will make the ongoing management of access rights much easier and more secure.
The data breach you prevent may be your own.

* RBAC vs. ABAC vs. ACL

Access control lists (ACL)  An ACL is a means of defining access rights by a given user or user group, to a specific object, such as a document.     
Attribute-based access control (ABAC) — ABAC, sometimes known as policy-based access control, can use a variety of attributes, including user department, time of day, location of access, type of access required, etc. to determine whether a user’s access request should be granted.    

#### RBAC implementation 

1. Inventory your systems
2. Analyze your workforce and create roles
3. Assign people to roles
4. Never make one-off changes
5. Audit

- - - 
