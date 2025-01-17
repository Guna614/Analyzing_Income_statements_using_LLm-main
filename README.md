# Analyzing_Income_statements_using_LLm-main

Analyzing Income Statements and Balance Sheets with LLM
PDF Table Extraction & Summarization
Project Overview
This project leverages cutting-edge technology LLM(Mistral-7B-Instruct-v0.2 model) from Hugging Face(using this llm because its for free of use) to simplify the complex process of analyzing financial documents such as income statements and balance sheets. The solution provides a comprehensive, AI-driven approach to extracting key financial insights, delivering human-readable summaries, and enabling faster, more informed decision-making for businesses and investors.


Through collaborative efforts, my team and I successfully streamlined the analysis of complex financial documents, overcoming challenges such as scalability, precision in data extraction, and real-time processing. This project is a testament to the transformative potential of AI in financial analytics.

✨ Key Features of the Project
📤 Upload PDFs
Easily upload your PDF documents using a seamless and user-friendly interface.

👀 Preview PDFs
View the content of your PDFs directly within the application before processing.

📊 Extract Tables
Automatically detect and extract complex tables from uploaded PDFs with precision.

📝 Summarize Tables
Generate AI-powered summaries of each extracted table, providing insightful overviews of financial data.

🧹 Automatic Cleanup
Maintain security and efficiency with automated cleanup processes that delete temporary files after processing.

⚡ AI-Driven Analysis
Identify key financial patterns, trends, and performance metrics effortlessly.

🌐 Real-Time Integration
Seamlessly integrate with financial platforms for real-time analysis and insights.

🔒 Data Security
Ensure compliance with financial data privacy standards to keep your information safe and secure.


🚀 Installation Steps
1️⃣ Clone the Repository
Clone the project repository to your local machine:

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
2️⃣ Set Up a Virtual Environment (Recommended)
Create and activate a virtual environment to manage dependencies:


# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows:
venv\Scripts\activate

# On macOS/Linux:
source venv/bin/activate

3️⃣ Install Dependencies
Install the required Python libraries using the requirements.txt file:

pip install -r requirements.txt
4️⃣ Set Up the Mistral-7B-Instruct-v0.2 Model

Download the Model:
Obtain the Mistral-7B-Instruct-v0.2 model from the official source or Hugging Face repository.
Place the downloaded model files in a directory, e.g., models/mistral-7b.

Install Necessary Model Libraries:

Ensure you have the required libraries for working with the model (e.g., transformers, accelerate):
pip install transformers accelerate

Configure the Model:
Update the configuration in your script to load the Mistral-7B-Instruct-v0.2 model:
from transformers import AutoModelForCausalLM, AutoTokenizer

model_name = "path/to/mistral-7b"
tokenizer = AutoTokenizer.from_pretrained(model_name)
model = AutoModelForCausalLM.from_pretrained(model_name)
5️⃣ Run the Application
Launch the application locally:
python main.py

6️⃣ Access the Application
Open your browser and navigate to:

http://localhost:5000
or the specified URL to interact with the user interface.


🚀 Usage Instructions
To start using the application, follow these steps:

🖥️ Launch the Application
Run the Streamlit app with the following command in your terminal:

streamlit run app.py
This will open the application in your default web browser.

🌟 How the Application Works
1️⃣ 📂 Upload Your PDF
Navigate to the sidebar of the application.
Use the file uploader to upload your PDF document (e.g., income statements, balance sheets).
2️⃣ 🔍 Preview the PDF
Once uploaded, the application will display a preview of your document.
You can verify the content before proceeding to analysis.
3️⃣ 📑 Extract Tables
The application will automatically detect and extract all tables from the uploaded PDF.
View extracted tables in expandable sections for easier navigation.
4️⃣ 📝 Summarize Tables
Click on the "Summarize" button for each extracted table.
The application uses the Mistral-7B-Instruct-v0.2 model to generate clear, concise summaries of financial data.
5️⃣ 💡 Gain Insights
Analyze the summaries to quickly understand the financial performance indicators, trends, and other critical insights.
Export or save the summarized results as needed.



Project Structure

pdf-table-extraction/  
├── app.py                 # Main Streamlit application file  
├── requirements.txt       # List of all project dependencies  
├── utils/                 # Utility modules for core functionalities  
│   ├── table_extraction.py    # Handles table detection and extraction  
│   └── summarization.py       # Implements AI-powered summarization logic  
├── README.md              # Project documentation file  
├── assets/                # (Optional) Stores images, icons, or other assets  
    └── icons/             # Directory for custom icons  



Dependencies
Streamlit

For building the web-based user interface.

pip install streamlit(Optional)
Transformers

For loading and working with the Mistral-7B-Instruct-v0.2 model.
pip install transformers
Accelerate

For efficient model inference and optimization.
pip install accelerate
PyPDF2

For handling PDF parsing and reading.
pip install PyPDF2
Pandas

For managing and processing extracted tabular data.
pip install pandas
Numpy

For numerical operations on data.
pip install numpy
Matplotlib/Plotly (Optional)

For visualizing trends and insights if required.
pip install matplotlib plotly
Python-Dotenv

For managing API keys and environment variables.
pip install python-dotenv
Tqdm (Optional)

For progress bars during table extraction or model inference.
bash
Copy
Edit
pip install tqdm
Requests (Optional)

For handling HTTP requests if external APIs are involved.
pip install requests

How to Install
Create a requirements.txt file with the following content:
streamlit
transformers
accelerate
PyPDF2
pandas
numpy
matplotlib
plotly
python-dotenv
tqdm
requests
Then install all dependencies in one go:
pip install -r requirements.txt


Contact
For any questions, feedback, or collaboration opportunities, feel free to reach out:

📧 Email: kgunakatakam614@gmail.com
