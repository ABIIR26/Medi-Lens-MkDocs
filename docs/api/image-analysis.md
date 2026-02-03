\# Image Analysis Flow



1\. Image uploaded from UI

2\. Validation and preprocessing

3\. AI model analysis

4\. Structured JSON response



Endpoint

`POST /analyze/document`



\### Request Body

| Field | Type | Description |

| :--- | :--- | :--- |

| `image` | base64/file | The medical document image. |

| `type` | string | `prescription` or `lab\_report`. |



\### Logic Flow

1\. \*\*Denoising:\*\* Removes background noise from the image.

2\. \*\*OCR Execution:\*\* Extracts raw text strings.

3\. \*\*Medical NER:\*\* Named Entity Recognition identifies drugs and dosages.

4\. \*\*Validation:\*\* Checks if the extracted drugs exist in the pharmaceutical database.



graph LR

&nbsp;   A\[User Document] -->|Upload Photo| B(Next.js Frontend)

&nbsp;   B -->|Post Image| C{API Gateway}

&nbsp;   C -->|Trigger| D\[AI Vision Model]

&nbsp;   D -->|Extract Text| E\[Medical NER Engine]

&nbsp;   E -->|Structured JSON| F(User Dashboard)

&nbsp;   F -->|Alerts| G\[Risk Warnings/Insights]

