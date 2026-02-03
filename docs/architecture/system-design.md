\# System Design



\# 🏗 High-Level Architecture

1\. \*\*Client Layer:\*\* User uploads data via Next.js.

2\. \*\*Processing Layer:\*\* Image is passed to a Python-based AI microservice.

3\. \*\*Persistence Layer:\*\* Structured data is stored in PostgreSQL (Supabase).

4\. \*\*Security Layer:\*\* Images are encrypted at rest in S3 Buckets.



\### 🔄 Data Lifecycle

Upload ➔ Pre-process ➔ AI Inference ➔ Structural Mapping ➔ UI Display ➔ User Verification.



Medi-Lens follows a modular architecture:

\- Frontend UI

\- API Layer

\- AI Processing

\- Database storage

