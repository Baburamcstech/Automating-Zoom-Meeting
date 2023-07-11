# Automating-Zoom-Meeting

#### In this project you will see the development and implementation of an automated system for creating Zoom meeting links.
---
---

### *Steps envloved in project* 
- First it reads the data from your gmail using imap.
  - it filters all the gmail according to subject and only takes the gmail containing meeting information.
  - Read the body of gmail and get the required details. 
  - map data into a python dictionary.
- automate the zoom using pyautogui to create a link.
- at last it sends the created link to the recipient gmail using smtp. 


---
---
### *Data flow diagram*
<br>
<img src="./Untitled%20Diagram.drawio.png" alt="drawing" width="500" height="450"/>

---
---
### *Settings for reading gmail using imap*
#### you need to generate app password in gmail
- steps  
  1. Log into your Gmail inbox.
  2. Click on your account icon and select the Manage your Google Account link.
  3. You will be redirected to your Google account page. Click on the Security tab in the left-hand side menu.
  4. Scroll down to the Signing in to Google section and select the App passwords option. If you don’t have two-step verification enabled, you should enable it to generate app passwords.
  You will be asked to provide your password again, and then you will be redirected to the App passwords page. 
  5. Under Select app, choose Mail, and under Select device choose Windows computer. If you use another device, please select the most relevant option.
  6. Once the app and device are selected, click on the Generate button. 
  7. Copy the password and paste the password in credentials.
---
---
### *Required mudules* 
- imaplib
- clipboard
- email
- pyautogui
- re
- time 
- smtplib
- yaml

<br>

#### to install any package type in command
```
pip install module_name
```


#### you need to edit in credentials and enter your gmail and password(got from app password above)
- example (example@gmail.com, example1234)

#### you can have list of receivers whom you want to send link.
