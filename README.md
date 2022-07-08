# Django Quickstart

## One liner: copy and paste the code below in your terminal > hit enter > type your project's name (no spaces) > hit enter


```
read PROJECT_NAME && \
mkdir $PROJECT_NAME && \
cd $PROJECT_NAME && \
mkdir $PROJECT_NAME && \
cd $PROJECT_NAME && \
python3 -m venv .$PROJECT_NAME && \
source .$PROJECT_NAME/bin/activate && \
python -m pip install django && \
django-admin startproject --template https://github.com/GuiFV/django-quickstart/archive/master.zip --name=Procfile,.env,pytest.ini $PROJECT_NAME . && \
pip install --prefer-binary -r requirements-dev.txt && \
git init && \
git add . && \
git commit -m 'Initial import' && \
heroku create $PROJECT_NAME && \
heroku config:set DEBUG=True SECRET_KEY=`cat .env | grep SECRET_KEY | cut -d = -f 2` ALLOWED_HOSTS="*" && \
git push heroku master
```
