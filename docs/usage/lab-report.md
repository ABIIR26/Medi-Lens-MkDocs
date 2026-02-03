\# Lab Report Analysis



Medi-Lens analyzes lab reports and:

\- Detects test names

\- Explains normal ranges

\- Highlights abnormal values



Medi-Lens supports a wide array of diagnostic panels.



\### How to Read the Results

\- \*\*Parameter:\*\* The name of the test (e.g., Creatinine).

\- \*\*Result:\*\* Your specific value.

\- \*\*Reference Range:\*\* The "Healthy" interval (e.g., 0.7 to 1.3 mg/dL).



\### Understanding Icons

\- 🟢 \*\*Normal:\*\* Result is within the safe range.

\- 🟡 \*\*Borderline:\*\* Result is at the edge of the range; lifestyle changes may be discussed.

\- 🔴 \*\*Critical:\*\* Result is significantly outside the range. \*\*Consult a professional immediately.\*\*



\# Supported Formats

\- Printed PDF reports.

\- Scanned physical documents.

\- Screenshots from patient portals.



sequenceDiagram

&nbsp;   participant User

&nbsp;   participant Frontend

&nbsp;   participant API

&nbsp;   participant AI\_Service

&nbsp;   participant DB



&nbsp;   User->>Frontend: Uploads Prescription

&nbsp;   Frontend->>API: POST /analyze (base64)

&nbsp;   API->>DB: Log Upload Event

&nbsp;   API->>AI\_Service: Process Image

&nbsp;   Note right of AI\_Service: Denoising \& OCR

&nbsp;   AI\_Service-->>API: Extracted Text (JSON)

&nbsp;   API->>API: Map Drugs to Database

&nbsp;   API-->>Frontend: 200 OK (Medical Insights)

&nbsp;   Frontend->>User: Display Parsed Results



