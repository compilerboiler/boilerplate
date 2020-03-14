---
date: 2020-02-16
title: python send email smtp
---
---
tags: ["python"]
date: 2020-02-16
title: python send email smtp
---
---
tags: ["python"]
date: 2020-02-14
title: python send email smtp
---
[SMTP (Simple Mail Transfer Protocol)](https://en.wikipedia.org/wiki/Simple_Mail_Transfer_Protocol) i.e., Simple Mail Transfer Protocol, which is a set of rules for transmitting from the source address to the destination address of the message, it an internet protocol.

The python smtplib provides a very convenient way to send e-mail. It smtp protocol for a simple package. You can use [pip to install it](https://pythonbasics.org/how-to-use-pip-and-pypi/).

Python create an SMTP object syntax is as follows:

```python
    import smtplib    
    smtpObj = smtplib.SMTP ([host [, port [, local_hostname]]])
```

Parameter Description:

* **Host:** SMTP server host. You can specify the host ip address or domain name such as: gmail, this is an optional parameter.
* **Port:** If you provide a host parameters, you need to specify the port number used by the SMTP service, under normal circumstances SMTP port number is 25.
* **Local_hostname:** If the SMTP on your local machine, you only need to specify the server address is localhost.

Python SMTP object to send mail using sendmail method syntax is as follows:

```python
    SMTP.sendmail (from_addr, to_addrs, msg [, mail_options, rcpt_options]
```

Parameter Description:

* **from_addr**: e-mail sender address.
* **to_addrs**: string list, send e-mail address.
* **msg**: Send a message

Here we must note that the third argument, msg is a string that represents the mail. 

We know that the email message is generally composed of a title, sender, recipient, message content, attachments. 

When sending mail, pay attention to msg format. This is a [string](https://pythonbasics.org/strings/), but the format is the format smtp defined in the protocol.

### smtp examples

The following is a Python to send mail using a simple example:

```python
    #!/usr/bin/python3
    import smtplib
    
    sender = 'from@fromdomain.com'
    receivers = [ 'to@todomain.com']
    
    message = "" "From: From Person <from@fromdomain.com>
    To: To Person <to@todomain.com>
    Subject: SMTP e-mail test
    
    This is a test e-mail message.
    "" "
    
    try:
       smtpObj = smtplib.SMTP('localhost')
       smtpObj.sendmail(sender, receivers, message)
       print("Successfully sent email")
    except SMTPException:
       print("Error: unable to send email")
```

##  send HTML formatted email Python

Python is different from the message transmitted HTML email message and sending plain text is set to the `MIMEText`. Specific code as follows:
```python
    import smtplib
    from email.mime.text import MIMEText
    mailto_list = [ "YYY@YYY.com"]
    mail_host = "smtp.XXX.com" # Set the server
    mail_user = "XXX" # Username
    mail_pass = "XXXX" # password
    mail_postfix = "XXX.com" # suffix Outbox
      
    def send_mail (to_list, sub, content): #to_list: Recipient; sub: Theme; content: the content of the message
        me = "hello" + "<" + mail_user + "@" + mail_postfix + ">" # hello herein can be arbitrarily set, on receipt, in accordance with the setting display
        msg = MIMEText(content, _subtype = 'html', _ charset = 'gb2312') # create an instance, the message format provided here html
        msg ['Subject'] = sub # Settings topic
        msg ['From'] = me
        msg ['To'] = ";". join(to_list)
        try:
            s = smtplib.SMTP()
            s.connect(mail_host) # smtp server connection
            s.login(mail_user, mail_pass) # login server
            s.sendmail(me, to_list, msg.as_string()) # Send e-mail
            s.close()
            return True
        except Exception, e:
            print(str(e))
            return False
    if __name__ == '__main__':
        if send_mail (mailto_list, "hello", "[ dev.to ](http://www.dev.to/)"):
            print("successfully sent")
        else:
            print("failed to send")
```

Or you can specify in the message body `Content-type: text / html`, the following example:

```python
    #!/usr/bin/python3
    import smtplib
    
    message = "" "From: From Person <from@fromdomain.com>
    To: To Person <to@todomain.com>
    MIME-Version: 1.0
    Content-type: text / html
    Subject: SMTP HTML e-mail test
    
    This is an e-mail message to be sent in HTML format
    
    <B> This is HTML message. </ B>
    <H1> This is headline. </ H1>
    "" "
    
    try:
       smtpObj = smtplib.SMTP('localhost')
       smtpObj.sendmail(sender, receivers, message)
       print("Successfully sent email")
    except SMTPException:
       print("Error: unable to send email")
```

## Python send mail with attachments

Send e-mail with attachments, you first create `MIMEMultipart()` instance and construction attachments, if there are multiple attachments, you can turn structure. Finally, smtplib.smtp sent.

```python
    from email.mime.text import MIMEText
    from email.mime.multipart import MIMEMultipart
    import smtplib
    
    # Create an instance with attachments
    msg = MIMEMultipart()
    
    # Structure Annex 1
    att1 = MIMEText(open (. 'example.zip', 'rb') read (), 'base64', 'gb2312')
    att1 ["Content-Type"] = 'application / octet-stream'
    att1 ["Content-Disposition"] = 'attachment; filename = "example.zip"' # where filename can be any write, write what name, what name appears in the message
    msg.attach (att1)
    
    # Structure Annex 2
    att2 = MIMEText(open (. 'example.txt', 'rb') read (), 'base64', 'gb2312')
    att2 ["Content-Type"] = 'application / octet-stream'
    att2 ["Content-Disposition"] = 'attachment; filename = "example.txt"'
    msg.attach (att2)
    
    # Plus headers
    msg ['to'] = 'YYY@YYY.com'
    msg ['from'] = 'XXX@XXX.com'
    msg ['subject'] = 'hello world'
    #send email
    try:
        server = smtplib.SMTP ()
        server.connect( 'smtp.XXX.com')
        server.login( 'XXX', 'XXXXX') # XXX user name, XXXXX is password
        server.sendmail(msg ['from'], msg ['to'], msg.as_string ())
        server.quit()
        print('transmission success')
    except Exception, e:
        print(str(e))
```

**Related links:**
* [Read email (with POP3)](https://pythonspot.com/read-email-pop3/)
* [Python smtplib module](https://docs.python.org/3.8/library/smtplib.html)

