# Data Storage

Each project in SRE has three storage folders.  

(i) Shared read-write: Workspace where everybody on the project has full access (edit/move/copy/delete). Everyone in the project can read-write in this folder. 

(ii) Shared read-only: A place where the data custodian can place data sets that are not to be changed by project team members. Data custodians have read-write access here and everybody else have read-only access. 

(ii) Personal: Each project team member has a personal folder in the SRE project where they have read-write privileges. Under personal folder there are two folders - Ingress and Egress. The data custodians/ingress and egress approvers access these folders to move in the requested files as part of data ingress or egress process. 

Please note that the data custodians have read-write access to the Researcher's personal folder in SRE.

### Storage structure for researcher 

Each researcher has access to three folders- one personal folder (with read-write access) and two shared project folders (with read-only and read-write access respectively). 

Click on the folder which have the data you need to work with. 

For data custodian’s folder structure, go to section () 

### Storage structure for Data Custodian 

The following are the list of folders a data custodian has access to: 

Project-rw - Shared project folder with read and write access.  
The content in this folder can be edited by the users who have access to it. 

Project-ro – Shared project folder with read only access.  
The data in this folder cannot be manipulated by anyone except data custodian. 

Project-personal – Personal folders of each user in the project will be listed in this folder.  
The data custodian can access any of these users’ personal folder to view/update/delete data in an SRE. 

Custodian – Only data custodian has access to this folder.  
When a data custodian ingress data directly, the uploaded files are moved into this folder and the data custodian can then move these files into project-rw, project personal (username) or egress-approver folder. 

Egress approver - Folder where all the egress request files land in. 
Both data custodian and egress approver have access to this folder. 

Ingress approver – Folder where all the ingress request files land in. 
Both data custodian and ingress approver have access to this folder. 
