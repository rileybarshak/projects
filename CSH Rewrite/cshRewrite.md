# CSH Rewrite
> **Project Type:** CSH project  
> **Project Description:** Rewrite & improvement of CSH services
> **Project Goal:** Follow better standards to improve functionality and maintainability 
> **Languages & Technologies:** GO, SQL, LDAP

## Rewrite Principles
- Use GO
- Use LDAP UUID instead of usernames (UID)
	- Don’t use LDAP when not needed (Audiophiler #61)
- Combine Services
	- Ex: Conditional + Packet + Profiles + EAC
- Add Docker Compose for every project

## First Step
### Conditional Rewrite
Project Lead: Ella (@ella)
- Rewrite Conditional in GO
- Integrate Packet, Profiles, EAC, etc


