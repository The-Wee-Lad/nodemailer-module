

# No-Reply Email Sender with Zoho SMTP

A simple Node.js script to send **no-reply** emails using **Zoho SMTP** with **Nodemailer**. The script provides real-time CLI feedback using **Ora** and supports text, HTML, and attachments.

make changes accordingly

## Features

- Send automated **no-reply** emails with Zoho SMTP
- Use **real-time CLI spinners** to track email sending progress
- Customizable email content with **text** and **HTML** formats
- Supports **attachments**
- Detailed **error handling** with response logs
- Ability to set custom email headers (like `replyTo`)

## Installation

1. Clone the repository or download the code:
   ```bash
   git clone https://github.com/your-username/no-reply-email-sender.git
   cd no-reply-email-sender
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Add your Zoho credentials in the script:
   - Replace `user` and `pass` in the `zohoMail` config with your Zoho account email and password.

## Usage

To send an email, call the `emailSenderWrapper()` function with appropriate arguments. Here’s an example:

```js
emailSenderWrapper(
  "recipient@example.com", // To email address
  "Test Email",            // Subject
  "This is a test email",  // Plain text content
  "<h1>This is an email</h1>", // HTML content
  []                       // Attachments (optional)
);
```
