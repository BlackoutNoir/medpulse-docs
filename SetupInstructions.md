# SETUP INSRUCTIONS

## Core Tech Stack (NOTE: Non-exhaustive list)
### Software Used/Alternatives 
#### FRONTEND
1) Next.js: building UI, leveraging SSR/SSG, and handling routing.
2) React: building components and managing state (Redux [ALT: ContextAPI/Jotai)].
3) Tailwind CSS: styling application.
#### BACKEND
1) FastAPI: web framework for building RESTful API to handle business logic and database interactions [ALT: Django/Flask].
2) SQLAlchemy: ORM to interact with the database (Pydantic for data validation/serialization).
#### DATABASE (BACKEND) 
1) PostgreSQL: database to store data.
#### ADDITIONAL TOOLS:
1) OAuth2: for authentication and securing API endpoints [ALT: JWT]
2) WebSocket or ZoomAPI: for real-time communication in virtual consultations.
3) Stripe/Paypal: payment processing. 

## FRONTEND
0) To install all dependencies, write (`npx install`)
1) Create NextJS App
- pnpm dlx create-next-app@latest [ALT: npx/yarn]
- Name: medpulse-ui-main
- TypeScript, ESLint, Tailwind CSS, SRC, App Router: Yes
- Customize Default Alias: No
- yarn dev (verify nextjs is working) 
3) Add ShadCN Component Library
- npx shadcn@latest init
- New York, Zinc, CSS Variables: Yes
- Result: src/lib/utils.ts


## DATABASE 
### DATABASE SETUP (LOCALLY)
- Download Postgresql from EDB (V17)
- Launch PGAdmin
- Right click Databases > Create Database > Name (e.g. QuizApplicationYT)
- Modify database.py.

## BACKEND
**References/Tutorials:**
1) Amigoscode: FastAPI Tutorial - Building RESTful APIs with Python: `https://youtu.be/GN6ICac3OXY?si=FpjatDYzA1XKp4nV`
2) Eric Roby: How to build a FastAPI app with PostgreSQL: `https://youtu.be/398DuQbQJq0?si=sTYQXNDHtAMFYwRL`

**To install all dependencies:**
- pip install -r requirements.txt

---

**Software Used/Alternatives:**
1) Python
2) FastAPI (API Backend)
- pip3 install fastapi "uvicorn[standard]"
4) Pydantic (Data Validation)
5) FastAPI Default SwaggerDocs (API endpoint testing) [ALTS: Thunder Client VSC Extension, Postman]
- localhost/docs (interactive)
- localhost/redoc (non-interactive API documentation)
6) SQLAlchemy (ORM)

---

**Virtual Environment:**
Instead of having all the dependencies on our computer, we can Silo these dependencies into each project. <br>
For instance, FASTAPI-POSTGRRESQL-PROJ directory, we can create an environment for this application without all these dependencies going to all our other python applications.
- `python3 -m venv env`
- `source env/bin/activate` OR `.\env\Scripts\activate` (windows)
- Install all required packages (e.g. pip install fastapi[all] psycopg2 - Replace fastapi[all] and psycopg2 with needed packages)
- Generate requirements file (every time new dependency is installed): `pip freeze > requirements.txt`
- Use requirements file to install required packages: `pip install -r requirements.txt`

---

**Setting up FastAPI:**
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

---

**Other installations:**
- python3 -m venv env
- source env/bin/activate (linux?) OR .\env\Scripts\activate (windows)
- where python (to confirm that you are in env path)
- pip3 install fastapi "uvicorn[standard]"
- pip3 install sqlalchemy psycopg2-binary


### Diagram: 
**FastAPI Diagram:** <br>
![image](https://github.com/user-attachments/assets/df6d5ef2-7907-4824-add7-568b614569f5)
