RAG Assistant for Design System Documentation
A Retrieval-Augmented Generation (RAG) assistant that helps teams quickly find and understand design system documentation.

This project is ideal for product teams, designers, and developers looking to quickly retrieve design guidelines, component usage instructions, accessibility notes, and more—all from one friendly chat interface.

🎯 About
This application allows you to:

Ask questions like “How do I implement a primary button in our design system?”

Get back the most relevant information from your design system docs.

Save time searching by leveraging vector search and an LLM to summarize and explain.

⚙️ Setup Instructions
1. Clone the repository
bash
Copy
Edit
git clone https://github.com/your-org/design-system-rag.git
cd design-system-rag
2. Create a virtual environment
bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
3. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
4. Configure environment
Create a .env file and add your API key:

ini
Copy
Edit
OPENAI_API_KEY=your_openai_key_here
(You can easily swap OpenAI for any other LLM you’d like — see config.py for setup options.)

5. Add your design system content
Put your design system markdown files or exported Confluence docs into the docs/ directory.

💻 Running Locally
Start the app:

bash
Copy
Edit
python app.py
Your assistant will be available at http://localhost:5001

☁️ Deploying
You can deploy this to Vercel or any other platform:

Push your code to GitHub.

Connect your repository to Vercel.

Set OPENAI_API_KEY in the Vercel environment settings.

Deploy!

📂 Project Structure
bash
Copy
Edit
.
├── app.py             # Flask application
├── docs/              # Design system source docs
├── templates/         # HTML templates
├── static/            # Static assets
├── requirements.txt   # Python dependencies
├── vercel.json        # Vercel config
├── .env               # Environment variables
📜 License
This project is for educational and internal use. Modify and adapt freely for your team’s design systems!

💬 Support
Questions? Feel free to reach out or open an issue in this repo.
