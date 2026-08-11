# Salesforce PDF Email Service

A Salesforce Apex-based email service that retrieves a PDF document and sends it as an email attachment using Salesforce's `Messaging.SingleEmailMessage` API.

## Features

- Send emails directly from Salesforce Apex
- Attach PDF documents to outgoing emails
- Gmail-compatible PDF attachment delivery
- Simple and reusable Apex service class
- Uses Salesforce's native email infrastructure

## Tech Stack

- Salesforce Apex
- Salesforce Developer Console
- Messaging.SingleEmailMessage
- HTTP Callouts
- Gmail

## Project Flow

1. User initiates email sending process.
2. Apex service retrieves the PDF document.
3. PDF is converted into a Blob.
4. Apex creates an email attachment.
5. Salesforce sends the email using `Messaging.sendEmail()`.
6. Recipient receives the PDF attachment in Gmail.

## Apex Service

The core implementation uses:

```apex
Messaging.SingleEmailMessage
Messaging.EmailFileAttachment
Messaging.sendEmail()
