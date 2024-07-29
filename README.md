# Email Analyzer

Email Analyzer is a web application that uses the Anthropic Claude API to analyze sales emails for professionalism and effectiveness. It provides a comprehensive evaluation of various aspects of the email, helping sales professionals improve their email communication.

## Features

- Analyzes sales emails for tone, clarity, structure, and effectiveness
- Provides detailed feedback on multiple aspects of the email
- Simple and intuitive web interface
- Powered by Anthropic's Claude AI model

## Requirements

- Python 3.7+
- Flask
- Anthropic Python library
- An Anthropic API key

## Obtaining an Anthropic API Key

To use this application, you'll need an API key from Anthropic. Here's how to get one:

1. Go to the Anthropic website (https://www.anthropic.com) and sign up for an account if you don't already have one.

2. Once logged in, navigate to the API section of your account dashboard.

3. Follow the prompts to create a new API key. You may need to provide some information about your intended use of the API.

4. Once created, you'll be shown your API key. Make sure to copy it and store it securely. You won't be able to see it again, although you can always generate a new key if needed.

5. Be aware that API usage may incur costs, so make sure to review Anthropic's pricing structure and terms of service.

Note: Keep your API key confidential and never share it publicly or commit it to version control systems.

## Setup

1. Clone the repository or download the source code.

2. Install the required Python packages:
   ```
   pip install flask anthropic
   ```

3. Set up your Anthropic API key as an environment variable:
   ```
   export ANTHROPIC_API_KEY=your_api_key_here
   ```
   Replace `your_api_key_here` with your actual Anthropic API key.

4. Save the provided `app.py` file in your project directory.

## Running the Application

1. Navigate to the project directory in your terminal.

2. Run the Flask application:
   ```
   python app.py
   ```

3. Open a web browser and go to `http://localhost:5000` to access the application.

## Usage

1. On the home page, you'll see a text area where you can paste your sales email content.

2. Click the "Analyze" button to submit the email for analysis.

3. The application will send the email to the Claude API for processing and display the results on a new page.

4. The analysis will cover the following aspects of your email:
   - Overall Impression
   - Tone and Professionalism
   - Clarity and Coherence
   - Structure and Organization
   - Opening and Closing
   - Call-to-Action
   - Personalization
   - Grammar and Spelling
   - Length and Conciseness
   - Suggestions for Improvement

5. Review the analysis and use the feedback to improve your email.

6. Click "Analyze Another Email" to return to the home page and analyze another email.

## Customization

You can modify the `app.py` file to customize the application:

- Adjust the HTML templates to change the appearance of the web pages.
- Modify the prompt in the `analyze_email()` function to change the aspects of the email being analyzed.
- Change the Claude model or other parameters in the API call to suit your needs.

## Security Note

This application is a basic example and may not be suitable for production use without additional security measures. Ensure you implement proper security practices, such as input validation and protection against common web vulnerabilities, before deploying this application in a production environment.

## License

This project is open-source and available under the MIT License.

## Acknowledgments

This application uses the Anthropic Claude API to provide AI-powered email analysis.
