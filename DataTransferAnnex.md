This section summarises in a comprehensive table all the actions to be performed in the case of Data Holders that will upload their data into a reference node.


<table>
  <tbody>
    <tr>
      <td colspan="3">
      <div align="center">Initial Assessment</div>
      </td>
    </tr>
    <tr>
      <th>Action</th>
      <th>Description</th>
      <th>Documents</th>
    </tr>
    <tr>
      <td>
        Submit an application for data incorporation use cases
      </td>
      <td>
        Complete the application for data incorporation use cases form for the Access Committee to evaluate the scientific relevance of your participation in EUCAIM as a data holder.
      </td>
      <td>
        <a href="#">External application form - Stakeholders - Data Holders</a>
      </td>
    </tr>
    <tr>
      <td>
        Complete the TIERs maturity level questionnaire
      </td>
      <td>
        Complete it to assess the readiness and compliance of your datasets and categorize them according to their maturity level (TIER 1, 2, or 3).
      </td>
      <td>
        <a href="https://dashboard.eucaim.cancerimage.eu/tier-maturity-level-questionnaire">https://dashboard.eucaim.cancerimage.eu/tier-maturity-level-questionnaire</a>
      </td>
    </tr>
    <tr>
      <td>
        Complete the DW maturity level questionnaire (only for clinical sites, as hospitals)
      </td>
      <td>
        Complete it to determine the current state of the hospital's Data Warehouse preparedness and maturity.
      </td>
      <td>
        <a href="https://dashboard.eucaim.cancerimage.eu/data-warehouse-maturity-questionnaire">https://dashboard.eucaim.cancerimage.eu/data-warehouse-maturity-questionnaire</a>
      </td>
    </tr>
  </tbody>
</table>


<table>
  <tbody>
      <tr>
      <td colspan="3">
      <div align="center">Ethical and Legal</div>
      </td>
    </tr>
    <tr>
      <th>Action</th>
      <th>Description</th>
      <th>Documents</th>
    </tr>
    <tr>
      <td>
        Provide documentation
      </td>
      <td>
        <ul>
            <li>Proof of legal representation and legal basis if necessary.</li>
            <li>A copy of a favorable ethical approval (if applicable).</li>
            <li>A report from the DPO confirming legal compliance.</li>
            <li>Any documents required under your national legislation</li>
            <li>Terms of Usage for the data.</li>
        </ul>
      </td>
      <td>
        <a href="#">D4.4 Final rules for participation report</a> (See Sections 4.4.1 (Legal requirements) and 4.4.2 (Ethical requirements for Data Holders)
      </td>
    </tr>
    <tr>
      <td>
        Data Transfer Agreement
      </td>
      <td>
        Fill-in and sign the DTA
      </td>
      <td>
        - <a href="#">Draft DTA</a>
      </td>
    </tr>
  </tbody>
</table>


<table>
  <tbody>
    <tr>
      <td colspan="3">
      <div align="center">Preliminaries</div>
      </td>
    </tr>
    <tr>
      <th>Action</th>
      <th>Description</th>
      <th>Documents</th>
    </tr>
    <tr>
      <td>
        Get Familiar with EUCAIM
      </td>
      <td>
        <ul>
            <li>Follow the EUCAIM training material and brief documents.</li>
            <li>Browse architecture and</li>
            <li>Watch webinars and videos.</li>
        </ul>
      </td>
      <td>
        - <a href="https://dashboard.eucaim.cancerimage.eu">https://dashboard.eucaim.cancerimage.eu</a><br/>
        - <a href="https://eucaim.gitbook.io/end-user-guide">https://eucaim.gitbook.io/end-user-guide</a><br/>
        - <a href="https://www.youtube.com/@EUCAIM">https://www.youtube.com/@EUCAIM</a><br/>
        - <a href="https://training.eucaim.cancerimage.eu">https://training.eucaim.cancerimage.eu</a>
      </td>
    </tr>
    <tr>
      <td>
        Request a EUCAIM User
      </td>
      <td>
        Request a EUCAIM User in the Dashboard through LS-AAI.
      </td>
      <td>
        - <a href="#">Registration of users in EUCAIM</a>
      </td>
    </tr>
  </tbody>
</table>


<table>
  <tbody>
    <tr>
      <td colspan="3">
      <div align="center">Data Preparation</div>
      </td>
    </tr>
    <tr>
      <th>Action</th>
      <th>Description</th>
      <th>Documents</th>
    </tr>
    <tr>
      <td>
        Extract Imaging and clinical data
      </td>
      <td>
        Use your own tools to extract the Medical Images and the clinical data
      </td>
      <td>
        N/A
      </td>
    </tr>
    <tr>
      <td>
        Annotate the data (optional)
      </td>
      <td>
        Use your own annotation tool or the one selected by EUCAIM (MITK). Convert the annotations into DICOM-SEG.
      </td>
      <td>
        - <a href="#">MITK (Medical Imaging Interaction Toolkit) Workbench</a><br/>
        - <a href="#">DicomSeg converter</a>
      </td>
    </tr>
    <tr>
      <td>
        Data de-identification
      </td>
      <td>
        Ensure that no identifiable information is present in the dataset. If your imaging data are not already de-identified, you may use the Lethe DICOM Anonymizer-
      </td>
      <td>
        - <a href="#">Lethe DICOM Anonymizer</a>
      </td>
    </tr>
    <tr>
      <td>
        Re-identification risk assessment (optional)
      </td>
      <td>
        Assess the risk of re-identification of patients based on your imaging metadata by checking hidden DICOM Tags.
      </td>
      <td>
        - <a href="#">Wizard</a>
      </td>
    </tr>
    <tr>
      <td>
        Data Quality Assessment (optional)
      </td>
      <td>
        You may check the accuracy and integrity of your imaging dataset
      </td>
      <td>
        - <a href="#">DICOM File integrity checker</a>
      </td>
    </tr>
  </tbody>
</table>


<table>
  <tbody>
    <tr>
      <td colspan="3">
      <div align="center">Data Uploading</div>
      </td>
    </tr>
    <tr>
      <th>Action</th>
      <th>Description</th>
      <th>Documents</th>
    </tr>
    <tr>
      <td>
        Provide Data Ingester Account Details
      </td>
      <td>
        Open a ticket in the helpdesk, select the "Reference nodes" group (or "Technical support team" if unavailable) and add a request with the title: "Create a data ingestion project in UPV" or "Create XNAT project in HealthRI" (depending on the Reference site), providing the name of the project, the username in EUCAIM who will manage it. An answer will be given soon.
      </td>
      <td>
        - <a href="https://help.cancerimage.eu">https://help.cancerimage.eu</a>
      </td>
    </tr>
    <tr>
      <td>
        Download and install the Data Ingestion tool
      </td>
      <td>
        Download the Data Ingestion tool for the UPV node and the Clinical Trial Processor (CTP) for HealthRI
      </td>
      <td>
        - <a href="#">QP-Insights Uploader</a> - <a href="#">CTP</a>.
      </td>
    </tr>
    <tr>
      <td>
        Request a user in the Reference node
      </td>
      <td>
        Choose the reference node where the data will be uploaded (only one):
        <ul>
          <li>UPV (login button, register through LS-AAI and ask for a "Data Ingester" account)</li>
        </ul>
      </td>
      <td>
        - <a href="#">Registration of users in UPV-eucaim-node</a>, <a href="https://www.health-ri.nl/en/services/xnat">https://www.health-ri.nl/en/services/xnat</a> - Health RI
      </td>
    </tr>
    <tr>
      <td>
        Upload Imaging Data
      </td>
      <td>
        Upload imaging data in the platform as described in the instructions (6.2.2 for UPV node and 6.2.3 for Health-RI).
      </td>
      <td>
        - <a href="#">User Guide for Data holders</a>, <a href="https://eucaim.gitbook.io/enduserguide/6-userguide4members">https://eucaim.gitbook.io/enduserguide/6-userguide4members</a>
      </td>
    </tr>
        <tr>
      <td>
        Upload clinical Data
      </td>
      <td>
        Once medical imaging data is uploaded, you can proceed with the clinical data. If the process of converting the clinical data is expected to be long, we encourage you to create an “image-only” dataset by skipping this step. Use the same tool as before for UPV and XNATpy for Health-RI. Data can be in CSV or JSON.
      </td>
      <td>
        - <a href="#">User Guide for Data holders</a>, <a href="https://eucaim.gitbook.io/enduserguide/6-userguide4members">https://eucaim.gitbook.io/enduserguide/6-userguide4members</a><br/>
        - <a href="#">QP-Insights Uploader</a>, <a href="https://bio.tools/qp-insights_uploader">https://bio.tools/qp-insights_uploader</a><br/>
        - <a href="#">XNATpy</a>, <a href="https://xnat.readthedocs.io/en/latest/">https://xnat.readthedocs.io/en/latest/</a>
      </td>
    </tr>
  </tbody>
</table>


<table>
  <tbody>
    <tr>
      <td colspan="3">
      <div align="center">Dataset Creation</div>
      </td>
    </tr>
    <tr>
      <th>Action</th>
      <th>Description</th>
      <th>Documents</th>
    </tr>
    <tr>
      <td>
        Create and Publish the Dataset
      </td>
      <td>
        The dataset has to be created according to the instructions in the Gitbook (section 6.2.2.3 for UPV and 6.2.3 for Health-RI).
      </td>
      <td>
        - <a href="#">User Guide for Data holders</a>
      </td>
    </tr>
    <tr>
      <td>
        Provide the dataset's metadata
      </td>
      <td>
        Provide the metadata of the datasets according to the EUCAIM schema. In case of doubts with the terminology, use textual descriptions.
      </td>
      <td>
        - <a href="#">EUCAIM Dataset metadata</a> or <a href="#">Molgenis excel template</a>
      </td>
    </tr>
    <tr>
      <td>
        Make a request of registry upload
      </td>
      <td>
        Create a helpdesk ticket on the category catalogue, providing the spreadsheet file with the metadata information. The helpdesk team will contact you back informing if the dataset has been properly registered or requesting more information.
      </td>
      <td>
        - <a href="https://help.cancerimage.eu">https://help.cancerimage.eu</a>
      </td>
    </tr>
    <tr>
      <td>
        Verify the entries in the catalogue
      </td>
      <td>
        Access the registry in the catalogue and verify the collection.
      </td>
      <td>
        <a href="https://catalogue.eucaim.cancerimage.eu/#/collection/&lt;&lt;identifier&gt;&gt;">https://catalogue.eucaim.cancerimage.eu/#/collection/&lt;&lt;identifier&gt;&gt;</a>
      </td>
    </tr>
  </tbody>
</table>
