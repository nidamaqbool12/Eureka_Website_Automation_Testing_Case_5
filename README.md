# Eureka_Website_Automation_Testing_Case_5

## Overview

This repository contains the Case_5 automation script. It is developed using Python and Selenium to automate Full Book Request ( Access_Type Free_To_Read Books) on the Eureka website. The script was developed in PyCharm IDE.

## Test Case Summary:

This positive test case verifies that a user can successfully access and download assigned Access_Typed_Free_To_Read books or  Access_Typed_Free_To_Read  book chapters from the Eureka Website. The user logs in with valid credentials and, after successful authentication, navigates from the homepage by hovering over the Publications menu and selecting By Title under the Books section, then selects a book from the list. If the selected book is assigned by the admin, the user is able to download the permitted content, either specific chapters or the complete book. The system ensures that only admin-assigned books or chapters are available for download, and the download process completes successfully.

## Folder Structure

<img width="619" height="351" alt="image" src="https://github.com/user-attachments/assets/573bee85-aef8-41f9-a023-ba8f99f894e8" />


## .env File

Install dotenv library:

pip install python-dotenv

Python Code to Load .env File:

import os
from dotenv import load_dotenv

Load .env file
load_dotenv(".env")

Variables
EMAIL = os.getenv("EMAIL")
PASSWORD = os.getenv("PASSWORD")
BASE_URL = os.getenv("BASE_URL")

.env File Content:

LOGIN CREDENTIALS
EMAIL=(Your Email)
PASSWORD=(Your Password)

SITE URL
BASE_URL=https://www.eurekaselect.com/

Creating Executable (.exe) File

Install PyInstaller:

pip install pyinstaller

Command to Create Executable:

pyinstaller --onefile --collect-all selenium Case_5.py
