# Python Mailgun Email Sender
This Python script allows you to send emails using the Mailgun API. It provides a simple function to send an email to a specified recipient with a subject and body. Below, you'll find instructions on how to set up and use this script.

## Prerequisites
Before you can use this script, you need to:
1. Have Python installed on your system.
2. Install the requests library using pip:
    ```bash
    pip install requests
    ```
## Setting Up
To set up the script for sending emails, you will need to obtain your Mailgun API endpoint and API key. Follow these steps:
1. Sign up for a Mailgun account if you haven't already.
2. Find your API key and API endpoint in your Mailgun dashboard.
3. Open the script and fill in your API endpoint and API key in the `MAILGUN_API_ENDPOINT` and `MAILGUN_API_KEY` variables, respectively.
Additionally, you need to specify the sender's email address in the `data` dictionary by filling in the 'from' key.

## Usage
To use the script to send an email, you will need to specify the recipient's email address, the subject of the email, and the body of the email. Here is an example of how to do this:
```python
to = "recipient@example.com"
subject = "Your Subject Here"
body = "The body of your email goes here."
send_email(to, subject, body)
```

Replace `recipient@example.com` with the actual recipient's email address, and customize the `subject` and `body` as needed.

## Running the Script
Once you have set up the script and filled in the necessary details, you can run the script using the following command:
```bash
python path/to/your_script.py
```

If the email is sent successfully, you will see a message saying "Email sent successfully!" If an error occurs, you will see "An error occurred while sending the email."

## Troubleshooting
- Ensure that your API key and API endpoint are correctly entered.
- Check the recipient's email address for typos.
- Review the Mailgun documentation for any changes to the API or limitations such as the allowed number of emails sent per day.
For more detailed information, refer to the [Mailgun API documentation](https://documentation.mailgun.com/en/latest/).

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.