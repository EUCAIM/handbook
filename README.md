

**Project title:** European Federation for Cancer Images

![image](figures/image0.png)

**Disclaimer**

The opinions stated in this report reflect the opinions of the authors and not the opinion of the European Commission.

All intellectual property rights are owned by the consortium of EUCAIM under terms stated in their Consortium Agreement and are protected by the applicable laws. Reproduction is not authorised without prior written agreement. The commercial use of any information contained in this document may require a licence from the owner of the information.

**Project acronym:** EUCAIM

**Grant Agreement:** 101100633

**Call identifier:** DIGITAL-2022-CLOUD-AI-02

**Data Holders EUCAIM Federation Handbook**

**Version:                 	0.6**

This version has the comments and changes accepted. A backuped version (0.5) with the suggestions and comments is available [here](https://docs.google.com/document/d/18Ue51ubiQmPGVJZ6XO5cL8QXL2Y8QG1X81BNh1FIw34/edit?usp=sharing)

Table of contents

[**1\. Introduction	3**](#1.-introduction)

[1.1. Purpose of the handbook	3](#1.1.-purpose-of-the-handbook)

[1.2. Overview of EUCAIM Data Federation, Data Holder’s Onboarding Workflow	3](#1.2.-overview-of-eucaim-data-federation,-data-holder’s-onboarding-workflow)

[**2\. Governance	5**](#2.-governance)

[2.1. Data governance	5](#2.1.-data-governance)

[**3\. Onboarding Process	6**](#3.-onboarding-process)

[3.1. Initial requirements and commitments	6](#3.1.-initial-requirements-and-commitments)

[3.2. Legal documents.	7](#3.2.-legal-documents.)

[**4\. Support and communication	9**](#4.-support-and-communication)

[4.1. Helpdesk and training resources	9](#4.1.-helpdesk-and-training-resources)

[4.1.1. EUCAIM training platform: Overview of courses and access	11](#4.1.1.-eucaim-training-platform:-overview-of-courses-and-access)

[**5\. Data Preparation process	12**](#5.-data-preparation-process)

[5.1. Tier 1 datasets	14](#5.1.-tier-1-datasets)

[5.2. Tier 2 and 3 datasets	16](#5.2.-tier-2-and-3-datasets)

[**6\. Option 1: Transfer to Reference Node	18**](#6.-option-1:-transfer-to-reference-node)

[6.1. Reference Nodes	18](#6.1.-reference-nodes)

[6.2. Transferring data to the nodes	19](#6.2.-transferring-data-to-the-nodes)

[**7\. Option 2: Setting up a Federated Node	21**](#7.-option-2:-setting-up-a-federated-node)

[7.1. Setting up the node	21](#7.1.-setting-up-the-node)

[7.1.1. Security and privacy considerations	22](#7.1.1.-security-and-privacy-considerations)

[7.1.2. Service Level Agreement	22](#7.1.2.-service-level-agreement)

[7.2. Tier 1 compliance	22](#7.2.-tier-1-compliance)

[7.3. Tier 2 compliance	23](#7.3.-tier-2-compliance)

[7.3.1. Node Registration and Deployment	25](#7.3.1.-node-registration-and-deployment)

[7.4. Tier 3 compliance	27](#7.4.-tier-3-compliance)

[**10\. References	28**](#10.-references)

[**ANNEX A: Data transfer checklist	29**](#annex-a:-data-transfer-checklist)

[**ANNEX B: Data Sharing checklist	32**](#annex-b:-data-sharing-checklist)


[^1]:  *Both folders can be found here: [Questionnaires](https://drive.google.com/drive/folders/1lflM8H_THJveNar3vS6_wAB9vfqEihhE)* *please, make sure to upload the completed questionnaires in the corresponding folder with your institution name first.*

[^2]:  *See ​​Deliverable [D4.4 Rules for Participation](https://drive.google.com/file/d/1QCAbv5nPpykos16-hmtKxFmb1h7YxP9B/view?usp=sharing), Sections 2, 4.1, and summarized in Table 2, [D5.6 Minimum Data Federation and Interoperability Framework](https://drive.google.com/file/d/1URY8jtofLQpokTh7Hzag2wFFV9r1d_fs/view?usp=sharing), Sections 4–6.*

[^3]:  *See [D5.6 Minimum Data Federation and Interoperability Framework](https://drive.google.com/file/d/1URY8jtofLQpokTh7Hzag2wFFV9r1d_fs/view?usp=sharing)* *section 3 and [https://eucaim.gitbook.io/architecture-of-eucaim/4.-detailed-architecture](https://eucaim.gitbook.io/architecture-of-eucaim/4.-detailed-architecture)* 

[^4]:  *See ​​Deliverable [D4.4 Rules for Participation](https://drive.google.com/file/d/1QCAbv5nPpykos16-hmtKxFmb1h7YxP9B/view?usp=sharing), section 4.3.1 (Data Transfer) and 4.3.2 (Data Sharing)., Sections 4–6*.

[^5]:  *See D4.4 [Final rules for participation report](https://drive.google.com/drive/folders/1dn1xQB9K7Fn3WzzqN5HRiQ7NiVwYt0yy) , Sections 4.1 and 4.4, D5.6 [Minimum Data Federation and Interoperability Framework](https://drive.google.com/drive/folders/1mzMxUBdah2a-Wm4jNJHqhDmB-ZSDCT_u), Section 3 (Federation Architecture and Agreements)\]*

[^6]:  *See D2.4 [Training Evaluation: Guidelines, Best Practices, Lessons Learned](https://drive.google.com/file/d/1hNCkrP8UutNiPexzAzpsdt3WDOwdVh66/view?usp=drive_link).*

[^7]:  See  D4.4 [Final rules for participation report](https://drive.google.com/drive/folders/1dn1xQB9K7Fn3WzzqN5HRiQ7NiVwYt0yy), Sections 4.4.1 (Legal requirements) and 4.4.2 (Ethical requirements for Data Holders).

[^8]:   You can generate a random key, for example, by running: $ head \-c 21 /dev/urandom

