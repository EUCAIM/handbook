# B. Annex: Data sharing checklist

This section summarises in a comprehensive table all the actions to be performed in the case of Data Holders that will deploy a federated node.

<h3 align="center">Initial Assessment</h3>

| Action | Description | Documents |  
| ---------- | ---------- | ---------- |
| Submit an application for data incorporation use cases. | Complete the application for data incorporation use cases form for the Access Committee to evaluate the scientific relevance of your participation in EUCAIM as a data holder. | - If you are a EUCAIM partner: [Call for use cases from EUCAIM partners](https://eu.jotform.com/233524103677050). <br>- If you are a EUCAIM stakeholder: [External application form - Stakeholders - Data Holders](https://form.jotform.com/251552461162350).| |
| Complete the TIERs maturity level questionnaire. | Complete it to assess the readiness and compliance of your datasets and categorize them according to their maturity level (TIER 1, 2, or 3). | - [https://dashboard.eucaim.cancerimage.eu/tier-maturity-level-questionnaire](https://dashboard.eucaim.cancerimage.eu/tier-maturity-level-questionnaire) |
| Complete the DW maturity level questionnaire (only for clinical sites, as hospitals) | Complete it to determine the current state of the hospital's Data Warehouse preparedness and maturity. | - [https://dashboard.eucaim.cancerimage.eu/data-warehouse-maturity-questionnaire](https://dashboard.eucaim.cancerimage.eu/data-warehouse-maturity-questionnaire) |

<br>

<h3 align="center">Ethical and Legal</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Provide documentation | <ul><li>Proof of legal representation and legal basis if necessary.</li><li>A copy of a favorable ethical approval (if applicable).</li><li>A report from the DPO confirming legal compliance.</li><li>GDPR compliance.</li><li>Data Protection Impact Assessment (DPIA), if applicable.</li><li>Evidence of an adequate anonymization/pseudonymization process that has been carried out</li><li>Documents demonstrating the security of the information system.</li><li>Any documents required under your national legislation.</li></ul> | - For more information see primarily the [Legal Handbook](https://docs.google.com/document/d/1U-RpFycjXEVP-4-l9ppveT654x78Dhlw/edit?tab=t.0), D4.4 [Final rules for participation report](https://drive.google.com/drive/folders/1dn1xQB9K7Fn3WzzqN5HRiQ7NiVwYt0yy) (See Sections 4.4.1 (Legal requirements) and 4.4.2 (Ethical requirements for Data Holders)) <br>- Find also here the template for the DPO report: [faq_DPO_template.docx](https://docs.google.com/document/d/1KHf1nlCxFB1BjhhQXHVo4zVSoOBorL_X/edit) |
| Data Sharing Agreement | Fill-in and sign the DSA | - [DSA](https://drive.google.com/file/d/1-UyQ02w0-shmRgQgp8L1ATWs1JEco3_Y/view?usp=drive_link) | 
| Define especial Access Conditions | A Document to be signed by the Data User that indicates the conditions under the Data User can access the data. | - [Draft Template](https://drive.google.com/file/d/1UMdDF52mXGHNIL0GegzfyuSBVfKCIl7d/view) |

<br>

<h3 align="center">Preliminaries</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Contact point for the negotiation (Only in federated nodes) | The LS-AAl details of the data holder delegate who will interact with the Data User through the negotiator. | - [Registration of users in EUCAIM LS-AAI.](https://drive.google.com/file/d/1EsFYxbzqpyYKggyeKrKKw3FkVecDby8P/view) |
| Get Familiar with EUCAIM | <ul><li>Follow the EUCAIM training material and brief documents.</li><li>Browse architecture and</li><li>Watch webinars and videos.</li></ul> | - [https://dashboard.eucaim.cancerimage.eu](https://dashboard.eucaim.cancerimage.eu)<br>- [https://eucaim.gitbook.io/end-user-guide](https://eucaim.gitbook.io/end-user-guide)<br>- [https://www.youtube.com/@EUCAIM](https://www.youtube.com/@EUCAIM)<br>- [https://training.eucaim.cancerimage.eu/](https://training.eucaim.cancerimage.eu/) |

<br>

<h3 align="center">Local Node (T1/2)</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Setup your local node | Deploy a node to host data and services to reach the desired interoperability level. | - Section 3.7 in [D5.6](https://drive.google.com/file/d/1URY8jtofLQpokTh7Hzag2wFFV9r1d_fs/view?usp=sharing) |
| Set up of the local catalogue (optional) | Deployment of a local instance of the catalogue. | - [Gitlab repository](https://gitlab.com/radiology/infrastructure/studies/eucaim/molgenis-emx2-eucaim) |
| Request a EUCAIM User | Request a EUCAIM User in the Dashboard. | - [Registration of users in EUCAIM](https://drive.google.com/file/d/1EsFYxbzqpyYKggyeKrKKw3FkVecDby8P/view) |

<br>

<h3 align="center">Data Preparation</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Extract the Imaging and clinical data | Use your own tools to extract the Medical Images and the clinical data | N/A |
| Annotate the data (optional) | Use your own annotation tool or the one selected by EUCAIM (MITK). Convert the annotations into DICOM-SEG. | - [MITK (Medical Imaging Interaction Toolkit) Workbench](https://bio.tools/mitk)<br>- [DicomSeg converter](https://hub.docker.com/r/mariov687/dicomseg) |
| Data de-identification | Ensure that no identifiable information is present in the dataset. If your imaging data are not already de-identified, you may use the EUCAIM Anonymizer. | - [Lethe DICOM Anonymizer](https://bio.tools/eucaim_dicom_anonymizer) |
| Re-identification risk assessment (optional) | Assess the risk of re-identification of patients based on your imaging metadata by checking hidden DICOM Tags. | - [Wizard](https://bio.tools/eucaim_wizard_tool) |
| Data Quality assessment (optional) | You may check the accuracy and integrity of your imaging dataset. | - [DICOM File integrity checker](https://bio.tools/dicom_file_integrity_checker_by_gibi230) |

<br>

<h3 align="center">Catalogue Population</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Create local catalogue (optional) | Data should follow the EUCAIM interoperability schema. | - [Sample file with the schema](https://docs.google.com/spreadsheets/d/19DDoFq-_Bj7wfEf5KjkISe13kS-W5EYQ/edit?usp=sharing&ouid=102741390744373897413&rtpof=true&sd=true) <br>- [End User Guide](https://github.com/EUCAIM/End-User-Guide/blob/main/6-UserGuide4Members) |
| Make a request for catalogue registration | Create a helpdesk ticket on the category catalogue, providing the link to the dataset in the local catalogue, if available, or the completed catalogue metadata spreadsheet. The helpdesk team will contact you back informing if the dataset has been properly registered or requesting more information. | -[https://help.cancerimage.eu](https://help.cancerimage.eu)<br>- [Catalogue metadata spreadsheet ](https://u.i3m.upv.es/9gx81) |

<br>

<h3 align="center">Federated Search</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Definition of Mapping to CDM Template (optional) | A mapping template of the mandatory and other significant attributes to the CDM should be defined. | Tables 14 and 15 in [D5.6](https://drive.google.com/file/d/1URY8jtofLQpokTh7Hzag2wFFV9r1d_fs/view?usp=sharing) |
| ETL process | The ETL tool should be applied to map the clinical and imaging data to the CDM. | - [https://bio.tools/eetl_toolset](https://bio.tools/eetl_toolset) |
| Development of Mediator Component (optional) | Develop a mediator to connect the local searching API with the federated explorer. | - Section 5.2.1 Dataset in a Federated Node. subsection "Guidelines for creating a mapping component" in [D5.6](https://drive.google.com/file/d/1URY8jtofLQpokTh7Hzag2wFFV9r1d_fs/view?usp=sharing) |
| Deployment of search components. | Deploy the Beam Proxy and the Focus query dispatcher. | - [https://eucaim.gitbook.io/enduserguide/6-userguide4members](https://eucaim.gitbook.io/enduserguide/6-userguide4members) |

<br>

<h3 align="center">Federated Processing</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Request registration in the federated explorer | Request the connection of the central instance of the federated search through a ticket in the helpdesk. | - [https://help.cancerimage.eu](https://help.cancerimage.eu) |
| Deployment of the FEM client | Deploy the container to run the service to interact with the federated processing. | - [https://gitlab.bsc.es/fl/fem-client](https://gitlab.bsc.es/fl/fem-client) |
| Deploy a federated computing node | Request technical support to the technical team through the helpdesk. | - [https://help.cancerimage.eu/](https://help.cancerimage.eu/) |

