# A. Annex: Data transfer checklist

This section summarises in a comprehensive table all the actions to be performed in the case of Data Holders that will upload their data into a reference node.

<h3 align="center">Initial Assessment</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Submit an application for data incorporation use cases | Complete the application for data incorporation use cases form for the Access Committee to evaluate the scientific relevance of your participation in EUCAIM as a data holder. | - If you are a EUCAIM partner: [Call for use cases from EUCAIM partners](https://eu.jotform.com/233524103677050). <br>- If you are a EUCAIM stakeholder: [External application form - Stakeholders - Data Holders](https://form.jotform.com/251552461162350  ).|
| Complete the TIERs maturity level questionnaire | Complete it to assess the readiness and compliance of your datasets and categorize them according to their maturity level (TIER 1, 2, or 3). | - [TIERs maturity level questionnaire](https://dashboard.eucaim.cancerimage.eu/tier-maturity-level-questionnaire) |
| Complete the DW maturity level questionnaire (only for clinical sites, as hospitals) | Complete it to determine the current state of the hospital's Data Warehouse preparedness and maturity. | - [Data Warehouse maturity level questionnaire](https://dashboard.eucaim.cancerimage.eu/data-warehouse-maturity-questionnaire) |

<br>

<h3 align="center">Ethical and Legal</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Provide documentation | <ul><li>Proof of legal representation and legal basis if necessary.</li><li>A copy of a favorable ethical approval (if applicable).</li><li>A report from the DPO confirming legal compliance.</li><li>Security compliance</li><li>GDPR compliance</li><li>Data Protection Impact Assessment (if applicable).</li><li>Any documents required under your national legislation</li><li>Evidence of an adequate anonymization/pseudonymization process that has been carried out</li><li>Terms of Usage for the data.</li></ul> | - For more information see primarily the [Legal Handbook](https://docs.google.com/document/d/1U-RpFycjXEVP-4-l9ppveT654x78Dhlw/edit?tab=t.0), D4.4 [Final rules for participation report](https://drive.google.com/drive/folders/1dn1xQB9K7Fn3WzzqN5HRiQ7NiVwYt0yy) (See Sections 4.4.1 (Legal requirements) and 4.4.2 (Ethical requirements for Data Holders)) <br> - Find also here the template for the DPO report: [faq_DPO_template.docx](https://docs.google.com/document/d/1KHf1nlCxFB1BjhhQXHVo4zVSoOBorL_X/edit) |
| Data Transfer Agreement | Fill-in and sign the DTA | - [DTA](https://drive.google.com/file/d/1TTuaFo4cWwomLJBtQbs_lkrBNFVSLH_L/view) | 

<br>

<h3 align="center">Preliminaries</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Get Familiar with EUCAIM | <ul><li>Follow the EUCAIM training material and brief documents.</li><li>Browse architecture and</li><li>Watch webinars and videos.</li></ul> | - [https://dashboard.eucaim.cancerimage.eu](https://dashboard.eucaim.cancerimage.eu)<br>- [https://eucaim.gitbook.io/end-user-guide](https://eucaim.gitbook.io/end-user-guide)<br>- [https://www.youtube.com/@EUCAIM](https://www.youtube.com/@EUCAIM)<br>- [https://training.eucaim.cancerimage.eu/](https://training.eucaim.cancerimage.eu/) |
| Request a EUCAIM User | Request a EUCAIM User in the Dashboard through LS-AAI. | - [Registration of users in EUCAIM](https://drive.google.com/file/d/1EsFYxbzqpyYKggyeKrKKw3FkVecDby8P/view) |

<br>

<h3 align="center">Data Preparation</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Extract Imaging and clinical data | Use your own tools to extract the Medical Images and the clinical data | N/A |
| Annotate the data (optional) | Use your own annotation tool or the one selected by EUCAIM (MITK). Convert the annotations into DICOM-SEG. | - [MITK (Medical Imaging Interaction Toolkit) Workbench](https://bio.tools/mitk)<br>- [DicomSeg converter](https://hub.docker.com/r/mariov687/dicomseg) |
| Data de-identification | Ensure that no identifiable information is present in the dataset. If your imaging data are not already de-identified, you may use the Lethe DICOM Anonymizer | - [Lethe DICOM Anonymizer](https://bio.tools/eucaim_dicom_anonymizer) |
| Re-identification risk assessment (optional) | Assess the risk of re-identification of patients based on your imaging metadata by checking hidden DICOM Tags. | - [Wizard](https://bio.tools/eucaim_wizard_tool) |
| Data Quality Assessment (optional) | You may check the accuracy and integrity of your imaging dataset | - [DICOM File integrity checker](https://bio.tools/dicom_file_integrity_checker_by_gibi230) |

<br>

<h3 align="center">Data Uploading</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Provide Data Ingester Account Details | Open a ticket in the helpdesk, select the "Reference nodes" group (or "Technical support team" if unavailable) and add a request with the title: "Create a data ingestion project in UPV" or "Create XNAT project in HealthRI" (depending on the Reference site), providing the name of the project, the username in EUCAIM who will manage it. An answer will be given soon. | - [https://help.cancerimage.eu](https://help.cancerimage.eu/) |
| Download and install the Data Ingestion tool | Download the Data Ingestion tool for the UPV node and the Clinical Trial Processor (CTP) for HealthRI | - [QP-Insights Uploader](https://bio.tools/qp-insights_uploader)<br>- [CTP](https://gitlab.com/radiology/infrastructure/data-curation-tools/ctp-standalone) |
| Request a user in the Reference node | Choose the reference node where the data will be uploaded (only one):<br><ul><li>UPV (login button, register through LS-AAI and ask for a "Data Ingester" account)</li><li>Health RI</li></ul> | - [Registration of users in UPV-eucaim-node](https://eucaim-node.i3m.upv.es/dataset-service/datasets?invalidated=false), <br>- [https://www.health-ri.nl/en/services/xnat](https://www.health-ri.nl/en/services/xnat) |
| Upload Imaging Data | Upload imaging data in the platform as described in the instructions (6.2.2 for UPV node and 6.2.3 for Health-RI). | - [User Guide for Data holders](https://eucaim.gitbook.io/enduserguide/6-userguide4members) |
| Upload clinical Data | Once medical imaging data is uploaded, you can proceed with the clinical data. If the process of converting the clinical data is expected to be long, we encourage you to create an “image-only” dataset by skipping this step. Use the same tool as before for UPV and XNATpy for Health-RI. Data can be in CSV or JSON. | - [QP-Insights Uploader](https://bio.tools/qp-insights_uploader)<br> - [XNATpy](https://xnat.readthedocs.io/en/latest/) |

<br>

<h3 align="center">Dataset Creation</h3>

| Action | Description | Documents |
| ---------- | ---------- | ---------- |
| Create and Publish the Dataset | The dataset has to be created according to the instructions in the Gitbook (section 6.2.2.3 for UPV and 6.2.3 for Health-RI). | - [User Guide for Data holders](https://eucaim.gitbook.io/enduserguide/6-userguide4members) |
| Provide the dataset's metadata | Provide the metadata of the datasets according to the EUCAIM schema. In case of doubts with the terminology, use textual descriptions. | - [EUCAIM Dataset metadata](https://docs.google.com/spreadsheets/d/1cj6YzIAchHnEKlH612gO91WzHfEOB4TbwBrl9a0kgE0/edit?usp=sharing) or [Molgenis excel template](https://docs.google.com/spreadsheets/d/19DDoFq-_Bj7wfEf5KjkISe13kS-W5EYQ/edit?usp=sharing&ouid=102741390744373897413&rtpof=true&sd=true) |
| Make a request of registry upload | Create a helpdesk ticket on the category catalogue, providing the spreadsheet file with the metadata information. The helpdesk team will contact you back informing if the dataset has been properly registered or requesting more information. | - [https://help.cancerimage.eu/](https://help.cancerimage.eu/) |
| Verify the entries in the catalogue | Access the registry in the catalogue and verify the collection. | - [https://catalogue.eucaim.cancerimage.eu/#/collection/<\<identifier>>](https://catalogue.eucaim.cancerimage.eu/#/collection/%3C%3Cidentifier%3E%3E) |

