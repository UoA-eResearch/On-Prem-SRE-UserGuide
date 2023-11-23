#On Premise (On-prem) SRE 

The On-prem SRE is built on our local Nectar infrastructure. Each environment consists of a set of modules/components that provide analytics (computation), data storage, access control, multi-tiered security, and a governance model in accordance with regulatory/project requirements. 

Every project in SRE is isolated from each other, as well as from the internet and the rest of the university services (e.g., no direct access to UniFiles) except where needed (e.g., Single Sign On, patching, etc.).  

#Data Storage  

Each project in SRE has three storage folders.  

i) Shared read-write: Workspace where everybody on the project has full access. Everyone in the project can read-write in this folder. 

ii) Shared read-only: A place where the data custodian can place data sets that are not to be changed by project team members. Data custodians have read-write access here and everybody else have read-only access. 

iii) Personal: Each project team member has a personal folder in the SRE project where they have read-write privileges. Please note that the data custodians can access this folder to move in the requested files as part of data ingress or egress process.  

#Definition of common terms used in SRE
 
UPI 

Data ingress 

Data egress 

Virtual desktop 

Airlock 

VPN 

Read-write 

Read-only 

Authy 

MFA 
