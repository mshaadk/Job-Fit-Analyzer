# Job Fit Analyzer
The Job Fit Analyzer is a web application designed to help job seekers analyze how well their resumes align with specific job descriptions. Powered by Google's Generative AI (Gemini), this tool acts as an intelligent Applicant Tracking System (ATS) and provides insightful feedback on resume match percentages, missing keywords, and a summary of how well the resume fits the job description.

## Features
- Upload a resume in PDF format.
- Input a job description in plain text.
- AI-powered evaluation of the resume against the job description.
- Displays matching percentage, missing keywords, and a profile summary.
- User-friendly interface built with Streamlit.

## How It Works
1. The user uploads a PDF resume and pastes the job description into the app.
2. The resume text is extracted using PyPDF2.
3. The extracted resume and job description are passed to Google Generative AI (Gemini).
4. The AI evaluates the resume based on the job description and returns a JSON-like response containing:
    - JD Match: Percentage match with the job description.
    - Missing Keywords: Important keywords missing from the resume.
    - Profile Summary: A summary of the resume's fit for the job.

## Tech Stack
- **Streamlit**: For building the interactive web application.
- **Google Generative AI (Gemini)**: Provides intelligent resume analysis and suggestions.
- **PyPDF2**: For extracting text from PDF files.
- **dotenv**: For securely managing environment variables.
- **Python**: The programming language used to implement the backend.

## Installation
1. Clone the repository:

```bash
git clone https://github.com/mshaadk/Job-Fit-Analyzer.git
```

2. Navigate to the project directory:

```bash
cd Job-Fit-Analyzer
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

4. Set up environment variables:

  - Create a .env file in the root directory.
  - Add your Google API Key:

```bash
GOOGLE_API_KEY=your_google_api_key
```

5. Run the Streamlit app:

```bash
streamlit run app.py
```

## Usage
1. Open the application in your browser by running the above command.
2. Paste the job description in the provided text area.
3. Upload your resume in PDF format.
4. Click the Submit button to analyze your resume.
5. The app will display the percentage match, missing keywords, and a profile summary.

## Project Structure
```bash
job-fit-analyzer/
│
├── app.py                # Main script for the Streamlit application
├── requirements.txt      # Project dependencies
├── .env                  # Environment variables (not included in repository)
├── README.md             # Project documentation
├── .gitignore            # Git ignore file
└── LICENSE.txt           # License File
```

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE.txt) file for details.

## Contributing
We welcome contributions! If you would like to contribute, feel free to open a pull request or issue for discussion.
