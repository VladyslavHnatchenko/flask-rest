# REST service on FLASK
_______________________________________________________________________

###### Set Up:
1. Clone repo: 
2. Go to folder: cd flask-app
3. Add virtualenv: python3 -m venv env
4. Activate virtualenv: source env/bin/activate
5. Install all libraries: pip install -r requirements.txt

_______________________________________________________________________

###### How to RUN:
1. Run locally: python3 app.py OR flask run
_______________________________________________________________________

###### How to TEST:

1. GET - all tasks:
curl -u chuck:python123 -i http://localhost:5000/todo/api/v1.0/tasks

2. GET - task by id:
curl -u chuck:python123 -i http://localhost:5000/todo/api/v1.0/tasks/2

3. POST - task with body:
curl -u chuck:python123 -i -H "Content-Type: application/json" -X POST -d '{"title":"Read a book"}' http://localhost:5000/todo/api/v1.0/tasks

4. PUT - update task:
curl -u chuck:python123 -i -H "Content-Type: application/json" -X PUT -d '{"done":true}' http://localhost:5000/todo/api/v1.0/tasks/2
_______________________________________________________________________
    