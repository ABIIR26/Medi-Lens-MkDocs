\# Tech Stack





The architecture is designed for speed, privacy, and high-accuracy AI inference.



\### Frontend \& UI

\- \*\*Next.js 14 (App Router):\*\* For server-side rendering and SEO-friendly documentation.

\- \*\*TypeScript:\*\* For strict type-safety across medical data structures.

\- \*\*Tailwind CSS + Shadcn/UI:\*\* To ensure a clean, accessible, and "medical-grade" aesthetic.



\### Backend \& Storage

\- \*\*Supabase:\*\* Used for PostgreSQL database management and user authentication.

\- \*\*Edge Functions:\*\* For low-latency API handling.



\### AI \& Processing

\- \*\*Vision Models:\*\* Utilizing models like Tesseract or specialized Transformers for text extraction.

\- \*\*NLP Engine:\*\* For mapping raw text to structured medical entities.

\### In Short 

\- Frontend: Next.js + TypeScript

\- Backend: API routes

\- AI: Image + text processing

\- Database: Supabase

\- Styling:  CSS



graph TD

&nbsp;   subgraph Client\_Side

&nbsp;       UI\[Next.js App]

&nbsp;       State\[React State/Context]

&nbsp;   end



&nbsp;   subgraph Server\_Side

&nbsp;       API\[Edge Functions]

&nbsp;       Auth\[Supabase Auth]

&nbsp;   end



&nbsp;   subgraph AI\_Engine

&nbsp;       OCR\[Vision Transformer]

&nbsp;       NLP\[Medical Logic Engine]

&nbsp;   end



&nbsp;   subgraph Storage

&nbsp;       DB\[(PostgreSQL Database)]

&nbsp;       S3\[Image Bucket]

&nbsp;   end



&nbsp;   UI <--> API

&nbsp;   API <--> Auth

&nbsp;   API --> OCR

&nbsp;   OCR --> NLP

&nbsp;   NLP --> API

&nbsp;   API <--> DB

&nbsp;   API --> S3



