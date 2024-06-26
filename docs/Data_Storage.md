# Data Storage

Each project in SRE has three storage folders.  

(i) **Shared read-write:** Workspace where everybody on the project has full access (edit/move/copy/delete). Everyone in the project can read-write in this folder. 

(ii) **Shared read-only:** A place where the data custodian can place data sets that are not to be changed by project team members. Data custodians have read-write access here and everybody else have read-only access. 

(iii) **Personal:** Personal folders of each user in the project will be listed in this folder. There are two subfolders under each project personal folder - ingress and egress folders.

After researcher's data ingress request is approved by the custodian/approver, the data is placed in the personal-ingress folder.

A researcher copies the data to be exported out of SRE in the personal-egress folder and requests egress and upon approval, the data is made availble to be downloaded.

The data custodian can access any of these users’ personal folder to view/update/delete data in an SRE. 

### Storage structure for Researcher 

Each researcher has access to the above three folders. Please note that the data custodians have read-write access to the Researcher's personal folder in SRE.

### Storage structure for Data Custodian 

The following are the list of folders a data custodian has access to: 

**Project-rw** - Shared project folder with read and write access.  
The content in this folder can be edited by the users who have access to it. 

**Project-ro** – Shared project folder with read only access.  
The data in this folder cannot be manipulated by anyone except data custodian. 

**Project-personal** – Each project team member has a personal folder in the SRE project where they have read-write privileges. 
Under personal folder there are two folders - Ingress and Egress. The data custodians/ingress and egress approvers access these folders to move in the requested files as part of data ingress or egress process. 

The data custodian can access any of these users’ personal folder to view/update/delete data in an SRE. 

**Custodian** – Only data custodian has access to this folder.  It has two sub-folders - ingress and egress

When a data custodian ingress data directly, the uploaded files are moved into ingress folder and the data custodian can then move these files into project-rw, project personal (username) or egress-approver folder. 

When a data custodian takes data out, they copy the output file in egress folder and requests egress and the data is available for download.

**Egress approver** - Folder where all the egress request files land in. 
Both data custodian and egress approver have access to this folder. 

**Ingress approver** – Folder where all the ingress request files land in. 
Both data custodian and ingress approver have access to this folder. 
