# Turbo Stealer

For **educational purposes** only, this program aims to spread awareness about how insecure some information is in our computers. Even if information like your passwords is encrypted, if someone gains access to your computer it will be at risk of being stolen. 

**Turbo Stealer** is a command line application programmed in python that is able to steal information from the computer running it. Currently, it is capable of stealing:
- **Emails** from:  
  - Windows registry
  - Windows credentials
  - Some Chromium based browsers
  - Some Firefox based browsers
- **Usernames and passwords** from:  
  - Some Chromium based browsers
  - Some Firefox based browsers

# Usage

1. Open **TurboStealer.exe**
1. A file containing the stolen information will be created.

# Settings

Some settings can be changed using command line arguments:  

- ```t```, ```target``` or ```targets```:  
  Changes the kind of information **Turbo Stealer** looks for. Multiple values can be selected by separating them with comas.  

  **Values:**  
  - ```m```, ```mail``` or ```mails```:  
  Enables looking for emails.
  - ```a```, ```account``` or ```accounts```:  
  Enables looking for usernames and passwords.

  **Default value:**  
  - ```mail,account```  

  **Examples of use:**  
  - ```TurboStealer.exe targets=mails```:  
  Only searches for emails.  
  - ```TurboStealer.exe targets=accounts```:  
  Only searches for accounts.  
  - ```TurboStealer.exe targets=mails,accounts```:  
  Searches for both emails and accounts.  

- ```s``` or ```save```:  
  Changes the file format used to save the information.  

  **Values:**  
  - ```t```, ```txt``` or ```text```:  
  Uses a TXT file to save the information.
  - ```j``` or ```json```:  
  Uses a JSON file to save the information.

  **Default value:**  
  - ```json```  

  **Examples of use:**  
  - ```TurboStealer.exe save=text```:  
  Uses a TXT file to save the information.
  - ```TurboStealer.exe save=json```:  
  Uses a JSON file to save the information.
