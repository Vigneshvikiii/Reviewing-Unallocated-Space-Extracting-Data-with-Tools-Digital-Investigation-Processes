# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes

## Name : Vignesh S

## Reg No : 212223230240

## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report

<img width="669" height="389" alt="image" src="https://github.com/user-attachments/assets/39d7a60f-ba3a-4c77-a824-bf8e1aa19b9f" />

<img width="1707" height="908" alt="image" src="https://github.com/user-attachments/assets/ad7b221b-918e-4a53-a52a-5a3c4d8e6861" />

<img width="1004" height="600" alt="image" src="https://github.com/user-attachments/assets/ea89ecd9-aea7-4378-9be8-a6047db75e71" />

<img width="1072" height="683" alt="image" src="https://github.com/user-attachments/assets/ddd49da6-61c2-4f27-94b9-7f734c6fd8fd" />

<img width="1078" height="676" alt="image" src="https://github.com/user-attachments/assets/c84ed199-ef4a-496f-9e2f-891f621ebaf9" />

<img width="1696" height="862" alt="image" src="https://github.com/user-attachments/assets/93724925-5668-4a4f-9457-48018252d2f5" />

<img width="1707" height="910" alt="image" src="https://github.com/user-attachments/assets/23cd1bd6-015b-468e-b8a4-4353b1e1a496" />

<img width="1726" height="892" alt="image" src="https://github.com/user-attachments/assets/60afe14f-778a-441d-99d2-9a5e2c89f66c" />

<img width="1477" height="886" alt="image" src="https://github.com/user-attachments/assets/6b52b6df-1092-4cdb-b09b-6642974196f4" />

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

