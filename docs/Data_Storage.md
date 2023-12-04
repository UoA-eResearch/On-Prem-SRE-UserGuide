#Data Storage

Each project in SRE has three storage folders.  

(i) Shared read-write: Workspace where everybody on the project has full access (edit/move/copy/delete). Everyone in the project can read-write in this folder. 

(ii) Shared read-only: A place where the data custodian can place data sets that are not to be changed by project team members. Data custodians have read-write access here and everybody else have read-only access. 

(ii) Personal: Each project team member has a personal folder in the SRE project where they have read-write privileges. Please note that the data custodians can access this folder to move in the requested files as part of data ingress or egress process.  