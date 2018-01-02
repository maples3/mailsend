# mailsend- a simple command-line email program
###### Because the name 'sendmail' is already taken :)

As you can probably guess from the name, this is a simple program that does
one thing- send emails.  It reads two files- a settings file and a file 
containing the message.

## Usage
```
usage: mailsend [-h] -s SETTINGS [-S SUBJECT] -t TEXTFILE

A very simple email client for sending messages

optional arguments:
  -h, --help            show this help message and exit
  -s SETTINGS, --settings SETTINGS
                        The email settings JSON file to use
  -S SUBJECT, --subject SUBJECT
                        The subject of the email
  -t TEXTFILE, --textfile TEXTFILE
                        The plain text file containing the message to send
```

## Settings format

It's a lot easier to show code than to describe it, so here's a sample:
```json
{
    "smtp_server": "smtp.gmail.com:587",
    "login_name": "your_gmail_account@gmail.com",
    "password": "1234pass",
    "from_address": "your_gmail_account@gmail.com",
    "to_address": "destination@example.com"
}
```
This isn't specific to Gmail accounts; it can work with any email service
that lets you send mail via SMTP (which I can't imagine any one that doesn't).
