Simple Resume Analyzer (AWS-Based)

This project allows users to upload a resume PDF, extracts the text using Amazon Textract, and sends it to an AI model (Amazon Bedrock or OpenAI) for feedback. The app returns 5 actionable suggestions to improve the resume.

## 🔧 Tech Stack
- AWS S3
- AWS Textract
- AWS Lambda
- Amazon Bedrock or OpenAI
- HTML / JavaScript (for upload form)

## 📁 Project Structure

- `frontend/`: Upload form (can be expanded to React)
- `lambda/`: Lambda function for processing and AI interaction
- `prompts/`: Prompt templates for LLM input
- `outputs/`: Sample outputs for testing
- `requirements.txt`: Dependencies for Lambda

## How It Works
1. User uploads a PDF resume via the frontend.
2. Resume is saved to S3.
3. Lambda is triggered → uses Textract to extract text.
4. Resume text is sent to an LLM (via Bedrock or OpenAI).
5. Suggestions are returned and displayed/saved.

Future Features
- Job description matching
- Resume scoring
- Tailored cover letter generation
