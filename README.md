# AI-Learning-Assistant
A Flask-based web application that transforms uploaded educational documents (PDF, PPT, images, text) into interactive learning materials, including detailed flashcards, quizzes, and a chatbot tutor.
Installation





Clone the Repository:

git clone <repository-url>
cd ai-learning-assistant



Set Up a Virtual Environment:

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate



Install Dependencies:

pip install flask google-generativeai pillow pypdf2 python-pptx



Set Environment Variables:





Create a .env file or set the GEMINI_API_KEY environment variable:

export GEMINI_API_KEY='your-gemini-api-key'  # On Windows: set GEMINI_API_KEY=your-gemini-api-key



Run the Application:

python app.py





Access the app at http://localhost:5000.

Usage





Upload a File:





Supported formats: PDF, PPT, PPTX, PNG, JPG, JPEG, GIF, TXT.



Maximum file size: 100MB.



Upload via the web interface to generate learning materials.



Features:





Summary & Explanation: View a concise summary and detailed explanation of the content.



Flashcards: Interactive flashcards with detailed answers, including formulas and diagram descriptions.



Quiz: 12-question quiz with explanations for answers.



Chatbot Tutor: Ask questions about the uploaded content for detailed, context-based responses.



Regenerate Content: Refresh learning materials without re-uploading.



Interact:





Navigate tabs (Summary, Flashcards, Quiz, Topics) to explore content.



Use the chat interface to ask questions about the material.

Project Structure





app.py: Main Flask application with routes for file upload, content generation, chatbot, and regeneration.



index.html: Frontend interface with Tailwind CSS for styling and JavaScript for interactivity.



uploads/: Temporary folder for uploaded files (auto-deleted after processing).

Requirements





Python 3.8+



Flask



google-generativeai



Pillow



PyPDF2



python-pptx

Notes





Ensure a valid Gemini API key is configured.



The application processes files locally and deletes them after extraction to save space.



Flashcards include comprehensive details (formulas, diagrams) for thorough learning.



The chatbot provides accurate, content-specific answers.

Troubleshooting





File Upload Errors: Ensure the file type is supported and under 100MB.



API Errors: Verify the Gemini API key and internet connection.



Content Issues: If no content is extracted, check if the file contains readable text or visuals.

License

MIT License
