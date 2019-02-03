#Entity Classes

##Department
a division of a university that students belong to. It purchases gift or pay cash to students. the responsibility for the department is to check the guidelines and sent the award request to proper officials.

###department attributes
..*Name: name of the department. For example: iSchool
..*Number of Award

##Guideline
A reference which define the type of funds and the level of approval. Department checks the guidelines. Other organizations (Provost office, Admin office and President/Dean/President) refer to the guidelines to do the next step.

###guidelines attributes
..*Category No: guideline category, there are 3 categories of funds.
..*Level of approval: determine who have the right to approve the award, for example: Dean, Provost, President.
..*Award amount: amount of the award, for instance: $50, $500, $1000
..*Special approved: Boolean, in category 3, the value of award which is less than $1000 and greater than $50 is special approved.  

##relationship

###checks
..*Scope note: a relationship between Department and Guideline. Department checks the guidelines and sent the award request to appropriate officials.
..*Domain: Department
..*Codomain: Guideline
..*Arity: 2 
..*Cardinality: 1-to-m

##refer to
..*Scope note: a relation between Department and Provost office, Admin office and President/Dean/Provost. These offices refer to the guidelines to determine the guideline category, the amount of award and who is take charge of the approving. 
..*Domain: Guideline
..*Codomain: Provost office, Admin office, President/Dean/Provost
..*Arity: 4
..*Cardinality: 1-to-1

