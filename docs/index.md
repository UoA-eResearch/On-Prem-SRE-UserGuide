#Introduction to SRE 
Secure research environment (SRE) provides a safe, remote computing environment for approved researchers to work collaboratively and analyse sensitive data augmented with layers of governance and auditing. The data which is brought into SRE and the analysed results which can be derived or exported from the environment is vetted by the authorised research team member to control the access to the sensitive information. Such monitored systems keep data safe while preventing misuse of data. 

!!The diagram will change!!

<figure markdown>
  ![diagram](img/diagram.png)
  <figcaption> </figcaption>
</figure>

``` mermaid
graph 
  %% definitions
  P1ingress(Project 1 Data Ingress);

  lake[(Datalake)];
  P1([Project 1 Service Work Bench]);
  P1W1{{Workbench - Rstudio}};
  P1W2{{Workbench - Matlab}};
  P1W3{{Workbench - Information Governance}};
  P1W1E1[Egress-bucket];
  P1W2E2[Egress-bucket];
  
  P1Egress([Egress App Project1]);
  P1Export(Export);
  
  %% relationships
  P1ingress --> |encrypted at rest| lake;
  
  lake --> P1;

  P1 -- PI --> P1W1;
  P1 -- Researcher 1 --> P1W2;

  P1W1 --> P1W1E1;
  P1W2 --> P1W2E2;

 P1W1E1 ----> P1Egress;
 P1W2E2 ----> P1Egress;
 P1Egress -->|Export after approval| P1Export;

 %% Information Governance relationships
 P1 -- PI / IG Lead  --> P1W3;
 P1W1E1 --> P1W3;
 P1W2E2 --> P1W3;
 P1W3 -.->|Permission applied after checks|P1Egress

```

-[SRE]: Secure Research Environment  
