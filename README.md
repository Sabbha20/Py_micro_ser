# Py_micro_ser

### Initial Setup
**Create Workspace**
```
mkdir Py_micro_ser
cd Py_micro_ser
```

**Activate Virtual Environment**
```
python3 -m venv .djenv  
source .djenv/bin/activate
```
*For Windows*
```
.djenv/Scripts/activate
```

**Install Packages**
```
pip3 install -r requirements.txt
```

**Create Project**
```
django-admin startproject admin
```

**Run Project**
```
cd admin
python3 manage.py runserver
```

**Create Docker-File**
```
touch Dockerfile docker-compose.yaml
```
**After setting both `Dockerfile` and `docker-compose.yaml`**
```
docker login
```
*Provide usename and password*
**or**
*Login to docker desktop terminal*
```
docker-compose up admin_db -d
docker-compose up
```