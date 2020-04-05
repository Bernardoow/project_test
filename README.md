# Steps to display the bug

1. go app folder => cd app/
2. initialize poetry => poetry shell 
3. install requirements => poetry install
4. run flask FLASK_APP=./app/app.py flask run
5. OK without bug.
6. Rename the file env to .env
7. Run flask again FLASK_APP=./app/app.py flask run
8. BUG !!!! Error: Failed to find Flask application or factory in module "app". Use "FLASK_APP=app:name to specify one.
9. Use the enviroment viriable => export FLASK_SKIP_DOTENV=1
10. Run again and OK without bug,