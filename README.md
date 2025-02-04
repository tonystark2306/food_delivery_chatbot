# Directory structure
backend: Contains Python FastAPI backend code db: Contains the dump of the database. You need to import this into your MySQL db by using MySQL Workbench tool dialogflow_assets: Contains training phrases etc. for our intents frontend: Contains website code

# Installation

Install the required modules:

```sh
pip install mysql-connector
pip install "fastapi[all]"
```
Or just run:
```sh
pip install -r backend/requirements.txt
```
Starting the FastAPI Backend Server
Go to the backend directory in your command prompt.
Run this command:
```sh
uvicorn main:app --reload
```
Ngrok for HTTPS Tunneling
To install ngrok, go to ngrok download and install the ngrok version that is suitable for your OS.
Extract the zip file and place backend/ngrok.exe in a folder.
Open Windows command prompt, go to that folder and run this command:
```sh
ngrok http 8000
```
NOTE: Ngrok can timeout. You need to restart the session if you see a session expired message.