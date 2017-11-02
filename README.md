# mailsend- a simple command-line email program
###### Because the name 'sendmail' is already taken :)

As you can probably guess from the name, this is a simple program that does
one thing- send emails.  It reads two files- a settings file and a file 
containing the message.

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
that lets you send mail via SMTP.
