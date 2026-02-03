# Local Setup



# Local Development Environment Setup

Follow these comprehensive steps to contribute to the Medi-Lens core.

### 📋 Prerequisites
- **Node.js:** v18.17 or higher.
- **Package Manager:** `npm` or `pnpm`.
- **Git:** For version control.

### 🛠 Installation Workflow
1. **Clone and Enter:**
   ```bash
   git clone [https://github.com/hridoy9011/Medi-lens.git](https://github.com/hridoy9011/Medi-lens.git)
   cd Medi-lens
Environment Variables: Create a .env.local and populate the following:

Code snippet
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_anon_key
AI_MODEL_ENDPOINT=your_ai_endpoint
Install Dependencies:

Bash
npm install
Boot the Environment:

Bash
npm run dev
Access the UI at http://localhost:3000

