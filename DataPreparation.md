# 5\. Data Preparation process {#5.-data-preparation-process}

The data compliance to the different tier levels can be performed progressively. The process starts with the extraction, annotation and de-identification of data and it is followed by three steps of standardisation, anonymisation check and quality check. [Figure 6](#fig_dataprep1) shows schematically those steps. 

![][image4]

[Figure 6](#figur_dataprep1): Steps for data preparation. Steps in bold are mandatory

The details of the steps will be provided in the following sections, but the outline is the following:

- **Raw data compliance to Tier 1** : Data has to be in the required format and de-identified. Quality and de-identification must be verified, the dataset must be registered in the public catalogue.  
- **Compliance to Tier 2**: Data required for the federated search must be standardised and de-identified. Quality and de-identification must undergo a more comprehensive verification process. Finally, data deposited in a federated node should be semantically aligned with the EUCAIM hyper-ontology and a query mediator component should be installed to run the search.  
- **Compliance to Tier 3** : Data must be standardized, follow the required structuring and be de-identified. Compliance to the EUCAIM common data model is required for all data. Quality and de-identification must be verified at the highest level.  Finally, data deposited in the federated node should be integrated in the materializer component.

For this purpose, several tools have been selected and developed in EUCAIM. [Figure 7](#fig_datatools) shows the main tools selected for this phase. Details on the downloading and usage of the tools are given in the following sections. 

[![][image5]](https://bio.tools/mitk)[![][image6]](https://hub.docker.com/r/mariov687/dicomseg)[![][image7]](https://bio.tools/dicom_file_integrity_checker_by_gibi230)[![][image8]](https://bio.tools/eucaim_dicom_anonymizer)![][image9][![][image10]](https://bio.tools/trace4medicalimagecleaning)  
![][image11][![][image12]](https://bio.tools/dicom_tags_extractor)[![][image13]](https://bio.tools/eetl_toolset)

[Figure 7](#figur_datatools): Data preparation tools. Click on the thumbnail for more information on the tool.

## 5.1. Tier 1 datasets {#5.1.-tier-1-datasets}

5.1.1. Requirements for your Tier 1 dataset

Tier 1 Data Holders must ensure that their data satisfy the following minimum requirements:

- Imaging data should be in DICOM format and associated annotations and segmentations, when available, should be in DICOM-SEG format. Specific cases will be considered if a DH has diagnostic images in different data formats.  
- All images should include a minimum set of imaging metadata and comply to the DICOM standard  
- Imaging data must be accompanied by a set of minimum clinical metadata.  
- Image and clinical data must be linked using the same patient ID.  
- No entity can exist more than once within your dataset.

The minimum metadata requirements for the imaging and clinical data are presented in this [document](https://docs.google.com/document/d/1uWE0faqNExufI-hb4b8rxDlD0lkVtLe0/edit).

5.1.2. Steps to prepare your Tier 1 dataset

The preparation of your dataset will follow the steps indicated in [Figure 6](#fig_dataprep1): 

* **Annotation (optional)**: you may want to annotate your imaging data, either by using your own tool. However, we recommend  using [**MITK (Medical Imaging Interaction Toolkit) Workbench**](https://bio.tools/mitk) to avoid the burden (and the risk) of additional conversion procedures.   
* **Format standardization (optional)**: it is recommended that  your imaging raw data are in DICOM format, and if applicable, that your annotations are in DICOM-SEG. If you need to convert annotation files to DICOM-SEG, you may use the EUCAIM [**DicomSeg converter**](https://hub.docker.com/r/mariov687/dicomseg) tool.   
* **De-identification** **(mandatory)**: you must ensure that no identifiable information (direct or indirect) is present in the dataset you will share. If your imaging data are not already de-identified, you may use the [**EUCAIM Anonymizer**](https://bio.tools/eucaim_dicom_anonymizer%20) ([Figure 8](#fig_dataanon)). In this case, you must ensure that the patient ID linking clinical and imaging data is identical and listed as the first variable in the clinical dataset for tabular data.  
  Special attention should be given to **embedded text** in images, that may contain patient-identifiable information, as well as **skull and head images** that pose a risk of patient re-identification. You may need to apply additional de-identification techniques to mitigate this risk.  
* **Re-identification risk assessment (optional)**: For assessing the risk of re-identification of patients based on your **imaging metadata** before sharing your dataset and further anonymizing your dataset through well known privacy models, you may use the [EUCAIM **Wizard tool**](https://bio.tools/eucaim_wizard_tool). Extraction of imaging metadata to feed the wizard tool is possible by using the [**DICOM tags extractor**](https://bio.tools/dicom_tags_extractor) tool ([Figure 8](#fig_dataanon)). Even if no automatic re-identification risk analysis on a combination of clinical and imaging metadata is possible at this Tier, you should carefully assess that no direct or indirect identifiers are present in your clinical data. 

![][image14]

[Figure 8](#figur_dataanon). Recommended de-identification process workflow

* **Data quality check (first level \- optional)** :   
  * You may check the **accuracy** and **integrity** of your imaging dataset using the [**DICOM File integrity checker**](https://bio.tools/dicom_file_integrity_checker_by_gibi230).  
  * In addition, **validity** assessment of 2D ultrasounds and mammographies **dataset** is possible using the [**Trace4MedicalImage cleaning**](https://bio.tools/trace4medicalimagecleaning) tool,  that detects and removes encapsulated text in DICOM files.  
* **Metadata registration in the public catalogue** **(mandatory)** : the table 4 below describes the steps to register your metadata.

More information on the EUCAIM tools available in [Figure 7](#fig_datatools).

| Action | Description | Support |
| :---- | :---- | :---- |
| Provide the dataset’s metadata in the spreadsheet template (Data Holder Template sheet) | The dataset schema can be downloaded from this [link](https://docs.google.com/spreadsheets/d/1cj6YzIAchHnEKlH612gO91WzHfEOB4TbwBrl9a0kgE0/edit?usp=sharing). In case of doubts with the terminology, use textual descriptions.  | A helpdesk ticket on the category of catalogue. |
| Make a request of registry upload | Create a helpdesk ticket on the category catalogue, providing the spreadsheet file with the metadata information. The helpdesk team will contact you back informing if the dataset has been properly registered or requesting more information. | Same procedure. |
| Verify the entries in the catalogue | Access the registry in the catalogue at the URL: [https://catalogue.eucaim.cancerimage.eu/\#/collection/](https://catalogue.eucaim.cancerimage.eu/#/collection/)\<\<identifier\>\>  | Same procedure. |

[Table 4](#table_tier1fedcat): Steps to submit the Metadata to the registry

## 5.2. Tier 2 and 3 datasets {#5.2.-tier-2-and-3-datasets}

5.2.1. Requirements for your Tier 2 and 3 dataset

Tier 2 Data Holders must ensure that their data satisfy the following minimum requirements:

- Imaging data should be in DICOM format and associated annotations and segmentations, when available, should be in DICOM-SEG format. Specific cases will be considered if a DH has diagnostic images in different data formats.

- All images should include a minimum set of imaging metadata and comply to the DICOM standard

- Imaging data must be accompanied by a set of minimum clinical metadata.

- Image and clinical data must be linked using the same patient ID.

- No entity can exist more than once within your dataset.

The minimum metadata requirements for the imaging and clinical data are presented in this [document](https://docs.google.com/document/d/1uWE0faqNExufI-hb4b8rxDlD0lkVtLe0/edit).

Tier 2-3 datasets must ensure their compliance to the EUCAIM’s Common Data Model according to the compliance level (the searchable variables for Tier 2 and full Common Data Model in tier 3). 

Compliance of your datasets with the EUCAIM **Common Data Model (CDM)** is recommended for Tier 2 nodes and mandatory for Tier 3 nodes. For Tier 2 data holders: if you do not wish to transform your data to the EUCAIM common data model, you can opt to implement a mapping component to interact with the federated search instead. Otherwise, EUCAIM offers dedicated tools that can help you with transforming your data to the EUCAIM CDM as described in Section 5.2.1 .

#### **EUCAIM Common Data Model and Hyperontology**

The [**EUCAIM Common Data Model**](https://eucaim.gitbook.io/eucaim-common-data-model/1.-introduction) defines a standardized structure for representing clinical and imaging metadata across the EUCAIM platform. It ensures that data contributed by different partners can be understood and used in a consistent way. 

**Key features:**

* It is based on the conceptual model of [mCode specification](https://ascopubs.org/doi/10.1200/CCI.20.00059) 

* The current version of the EUCAIM CDM Data Dictionary is available [here](https://docs.google.com/spreadsheets/d/1ox9PdvfCDxpDmEnFzC1M6OFhUhXpjQzg/edit?usp=sharing&ouid=115998150174651530097&rtpof=true&sd=true).

* Supports multimodal data (i.e. imaging and clinical).

* Facilitates efficient querying, tool compatibility, and federated analysis and learning.

The [**EUCAIM** **hyperontology**](https://hyperontology.eucaim.cancerimage.eu/) is a common semantic meta-model that supports and maintains semantic interoperability and ensures consistent mapping and harmonization with the EUCAIM CDM entities (tables and attributes). It provides rich context, making it easier for users and tools to interpret, search, and reason over the data. In addition, the EUCAIM Hyperontology connects the CDM’s data fields to standardized biomedical concepts (i.e. terminology-binding) to verify that the data elements represented in the EUCAIM CDM are semantically aligned with the knowledge (concepts and object/data properties) described in the hyper-ontology. This ensures a coherent interpretation and understanding of data between the hyper-ontology and CDM. 

#### **Why it is important:**

As a data holder, understanding the CDM and hyperontology is essential for:

* **Mapping your data correctly**: Ensuring your local dataset aligns with EUCAIM standards.

* **Using tools effectively**: Tools in the EUCAIM ecosystem rely on the CDM to operate correctly.

* **Supporting reproducibility and scalability**: Harmonized data makes it easier to run federated analysis and integrate new tools.

5.2.2 Steps to prepare your Tier 2 or Tier 3 dataset

The preparation of your dataset will follow the steps indicated in [Figure 6](#fig_dataprep1): 

* **Annotation (optional)** : you may want to annotate your imaging data, either by using your own tool, or using the EUCAIM annotation tool [**MITK (Medical Imaging Interaction Toolkit) Workbench**](https://bio.tools/mitk).   
* **Format standardization (mandatory for Tier 3\)** : you need to make sure that your imaging raw data are in DICOM format, and if applicable, that your annotations are in DICOM-SEG. If you need to convert annotation files to DICOM-SEG, you may use the EUCAIM [**DicomSeg converter**](https://hub.docker.com/r/mariov687/dicomseg) tool. As for your clinical data, they must be structured in a tabular format with patient ID as first variable.  
* **De-identification** **(mandatory)**: you must ensure that no identifiable information (direct or indirect) is present in the dataset you will share. If your imaging data are not already de-identified , you may use the [**EUCAIM Anonymizer**](https://bio.tools/eucaim_dicom_anonymizer%20) ([Figure 7](#bookmark=kix.br72yai62sd4)).   
  Special attention should be given to **embedded text** in images, that may contain patient-identifiable information, as well as **skull and head images** that pose a risk of patient re-identification. You may need to apply additional de-identification techniques to mitigate this risk.  
* **Data quality check (second level \- optional)** :   
  * You may use the [**DIQCT**](https://bio.tools/data_integration_quality_check_tool_diqct) to help you assess various aspects of your dataset’s quality, both for imaging and clinical data, such as its **completeness, uniqueness, validity, consistency, integrity.**   
  * You may also check the **accuracy** and **integrity** of your imaging dataset using the [**DICOM File integrity checker**](https://bio.tools/dicom_file_integrity_checker_by_gibi230).  
  * In addition, **validity** assessment of 2D ultrasounds and mammographies **dataset** is possible using the [**Trace4MedicalImage cleaning**](https://bio.tools/trace4medicalimagecleaning) tool,  that detects and removes encapsulated text in DICOM files.  
* **Data conversion to EUCAIM Common Data Model (mandatory)**

  Transformation of the clinical and imaging datasets in accordance with the EUCAIM CDM is recommended for Tier 2 nodes and mandatory for Tier 3 nodes. Tier 2 nodes can opt instead to implement a custom mapping component to interact with the federated search service.   
  The transformation step requires:

  a) For your imaging dataset : the extraction of the DICOM metadata . The [**DICOM tags extractor**](https://bio.tools/dicom_tags_extractor)  can be used to this end.

  b) For clinical dataset : the mapping between the source clinical metadata and the EUCAIM CDM. 

  c) the actual transformation of all the clinical and imaging data to a format compliant with the EUCAIM CDM through the use of the [**EUCAIM ETL**](https://bio.tools/eetl_toolset). 

* **Re-identification risk assessment (optional)**: For assessing the risk of re-identification of patients based on your **imaging metadata** before sharing your dataset and further anonymizing your dataset through well known privacy models, you may use the EUCAIM **Wizard tool**. Extraction of imaging metadata to feed the wizard tool is possible by using the [**DICOM tags extractor**](https://bio.tools/dicom_tags_extractor) tool (Figure 7). Even if no automatic re-identification risk analysis on a combination of clinical and imaging metadata is possible at Tier 1, you should carefully assess that no direct or indirect identifiers are present in your clinical data. The Wizard tool should be applied on both imaging and clinical data, with  the latter having to follow  only on datasets following the EUCAIM CDM (Tiers 2 and 3).  
* **Metadata registration in the public catalogue (mandatory)**: Please refer to [Table 4](#tab_tier1fedcat) for the steps to register your metadata.


More information on the EUCAIM tools available in [Figure 7](#fig_datatools).
