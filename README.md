## Run the project

Make sure you are in main_backend directory

Make a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment:
* linux:


```bash
source venv/bin/activate
```


* windows:
```bash
venv\Scripts\activate
python.exe -m pip install --upgrade pip
```

Install the required packages:
```bash
pip install -r requirements.txt
```

Make a copy of the example environment variables file and call it `.env`:
```bash
copy .env.example .env
```
Edit the environmental variables and enter your variables 

NOTE: if left without edit the application will run but PayPal payment won't work

Run migrations:
```bash
python manage.py migrate
```

Create superuser:
```bash
python manage.py createsuperuser
```

Run server:
```bash
python manage.py runserver
```

now you have the server running go to 
http://127.0.0.1:8000/api/v1/
and see the API

you can go to http://127.0.0.1:8000/admin
to sign in as a superuser then go to the api url.
