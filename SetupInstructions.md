# SETUP INSRUCTIONS

## FRONTEND

## BACKEND
Software Used/Alternatives:
1) Python
2) FastAPI (API Backend)
3) Pydantic (Data Validation)
4) FastAPI Default SwaggerDocs (API endpoint testing) [ALTS: Thunder Client VSC Extension, Postman]
- localhost/docs

Setting up FastAPI:
1) Make sure Python is Installed
  - `python --version`. If it is installed, you will see something like `Python 3.10.0`
2) Install Python PIP on Windows [`REF: https://www.geeksforgeeks.org/how-to-install-pip-on-windows/`]
- Save this python file where Python is installed `https://bootstrap.pypa.io/get-pip.py`
- `python get-pip.py`
- `pip --version`
3) Install FastAPI and Uvicorn [`REF: https://youtu.be/GN6ICac3OXY?si=FpjatDYzA1XKp4nV`]
- `pip3 install fastapi "uvicorn[standard]"`
4) Run Server
- Create main.py and add app instance.
- `uvicorn main:app --reload`


### Diagram: 
**FastAPI Diagram:** <br>
![image](https://github.com/user-attachments/assets/df6d5ef2-7907-4824-add7-568b614569f5)
