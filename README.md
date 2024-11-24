# Fraudulent Email Identifier – Comprehensive Overview
The Fraudulent Email Identifier is a multi-platform solution designed to safeguard users from email-based scams such as phishing, spoofing, and other fraudulent attempts. By combining a web application and a browser extension, the system empowers users to evaluate emails efficiently, minimizing their exposure to cyber threats.

## Core Components

- **Web Application**: 
- Built with Flask, a lightweight Python web framework, ensuring a user-friendly interface and fast processing.
- Users can manually input email attributes like sender address, subject line, and body text.
- The system provides an instant detection report that highlights red flags, such as:
- Suspicious URLs: Links redirecting to unexpected or unknown domains.
- Impersonated Senders: Sender addresses that mimic legitimate organizations.
- Urgent Language: Phrases like “Act Now” or “Your account will be locked.”
- Uses machine learning (optional enhancement) or rule-based logic to evaluate email patterns.

- **Browser Extension:**:
- Designed as a Chrome extension, with planned compatibility for other browsers.
- Enables users to check emails directly from platforms like Gmail or Outlook without leaving their inbox.
- Analyzes emails with a single click, providing real-time warnings for potentially fraudulent content.

- **Rule-Based Detection**: Checks emails for suspicious links, sender addresses, and urgent language.

## How It Works
1. Input Data: Users enter the email’s sender address, subject, body text, and any embedded links.
2. Predefined Rules: The system cross-checks the email against a set of predefined rules, such as:
- Use of common phishing domains (e.g., “bit.ly” or typos in legitimate domains like "paypa1.com").
- Anomalies in sender information (e.g., mismatched “From” and “Reply-To” addresses).
3. Triggers for psychological pressure, such as deadlines or penalties.
- Results: A report is generated with a confidence score (e.g., 80% likelihood of phishing) and an explanation of flagged issues.

### Requirements

- Python
- Flask
- Flask-cors

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/pranjalsingh03/phising-email-detector.git
    cd phishing-email-detector
    ```

2. Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Flask application:
    ```bash
    python app.py
    ```

4. Open your browser and go to `http://127.0.0.1:5000/`.

### File Structure

- `app.py`: The main Flask application.
- `templates/index.html`: The HTML template for the web application.
- `static/styles.css`: The CSS file for styling the web application.
- `detector/rule_factory.py`: Contains the logic for the phishing detection rules.

### Usage

1. Open the web application in your browser.
2. Enter the email details (From, Subject, Body).
3. Click "Check Email" to get the phishing detection report.
4. To clear the report, click "Clear Report".

## Chrome Extension

### Installation

1. Open Chrome and go to `chrome://extensions/`.
2. Enable "Developer mode" using the toggle switch in the top right.
3. Click "Load unpacked" and select the `chrome_extension` directory from the repository.

### Usage

1. Open Gmail in Chrome.
2. Click the Phishing Email Detector icon in the Chrome toolbar

## Contributors
Ashish S - 
Final Year Student - Presidency University


