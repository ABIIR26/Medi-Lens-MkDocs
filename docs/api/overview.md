\# API Overview



The API processes medical images and returns structured results.



It acts as the bridge between frontend and AI services.



The Medi-Lens API is built on REST principles, returning JSON-encoded responses and using standard HTTP response codes.



\### Authentication

Most endpoints require a Bearer Token provided by Supabase Auth:

`Authorization: Bearer <your\_token>`



\### Rate Limiting

\- \*\*Free Tier:\*\* 50 requests/hour.

\- \*\*Developer Tier:\*\* 5000 requests/hour.



