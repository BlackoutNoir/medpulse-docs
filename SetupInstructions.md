# SETUP INSRUCTIONS

## FRONTEND

## BACKEND
References:
1) Amigoscode: FastAPI Tutorial - Building RESTful APIs with Python: `https://youtu.be/GN6ICac3OXY?si=FpjatDYzA1XKp4nV`
2) Eric Roby: How to build a FastAPI app with PostgreSQL: `https://youtu.be/398DuQbQJq0?si=sTYQXNDHtAMFYwRL`


Software Used/Alternatives:
1) Python
2) FastAPI (API Backend)
- pip3 install fastapi "uvicorn[standard]"
4) Pydantic (Data Validation)
5) FastAPI Default SwaggerDocs (API endpoint testing) [ALTS: Thunder Client VSC Extension, Postman]
- localhost/docs (interactive)
- localhost/redoc (non-interactive API documentation)
6) SQLAlchemy (ORM)

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

Other installations:
- python3 -m venv env
- source env/bin/activate
  - instead of having all the dependencies on our computer, we can Silo these dependencies into each project.
  - For instance, FASTAPI-POSTGRRESQL-PROJ directory, we can create an environment for this application without all these dependencies going to all our other python applications.
- pip3 install fastapi "uvicorn[standard]"
- pip3 install sqlalchemy psycopg2-binary


### Diagram: 
**FastAPI Diagram:** <br>
![image](https://github.com/user-attachments/assets/df6d5ef2-7907-4824-add7-568b614569f5)
