# Devin (3d-printer PC) Accountization
> **Project Type:** CSH Project
> **Project Goal:** Improve 3d-printing system
> **Languages & Technologies:** CSH LDAP, FreeIPA, pGina, Kerberos

### Problem
The 3D Printers are having problems much more often than they should be... this is costing CSH not only our time, but our money as well. While being confident is great, if you don't know how to use something properly, you shouldn't. Unfortunately, this does not always happen, and as a result our printers break far more frequently than they should. This will soon become an even larger issue once we get our hands on the two new printers we are spending $3,000 on... Additionally, the desktop and software are filled with people's individual projects, cluttering the space and making it more difficult to navigate.


### Solution
Like User Machines, users will sign-in to the 3D PC using their CSH login. If the user has the LDAP role, they will be given access to 3d-printers, if not, they will not. These creds would be earned by attending a 3D-printing seminar and passing a 3D-printing quiz (similar to how you gain access to the project room as a whole). This would ensure everyone using the printers is at least educated on basic use, which (in my opinion) would reduce the number of mistakes made drastically. Additionally, individual accounts would allow for users to keep their files private and reduce clutter among shared software. 


### Default Apps
**General:**
* MS Edge

**Slicers (creds required):**
* Bambu Studio
* PrusaSlicer
* MakerBot Print

**CAD:**
* Autodesk Fusion
* KiCad 

 
***


### Relevant Docs

https://wiki.csh.rit.edu/wiki/LDAP	-	ldap setup
https://wiki.csh.rit.edu/wiki/FreeIPA#Eveng 	-	Windows User Machine & setup guide
* pGina/FreeIPA (https://github.com/pgina/pgina/wiki)

Kerberos Setup Required for pGina/FreeIPA
- auth mechanism
- https://wiki.csh.rit.edu/wiki/Kerberos