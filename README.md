# Simple Notes App
This is a simple notes app built with React and Django.

## Requirements
1. Python 
2. Node.js
3. React

## Installation
1. Clone the repository
```
git clone https://github.com/Hitstar53/notesapp.git
```
2. Create a virtual environment and activate it
```
virtualenv venv
venv\Scripts\activate  
```
3. Install the requirements
```
pip install -r requirements.txt
```
4. Run the server
```
python manage.py runserver
```

## Frontend - React
5. Open another terminal and navigate to the mynotes directory
```
cd mynotes
```
6. Install the dependencies
```
npm install
```
7. Run the app
```
npm start

```
```
ubuntu instance
-----------------------------------------
install git, docker , python, nginx

apt-get update
apt install nginx

Installation

docker build -t notes-app .

docker run -d -p 8000:8000 notes-app:latest

```
```
---reverse proxy nginx---- (to global access)

curl -L http://127.0.0.1:8000

cd /etc/nginx/sites-enabled/

go to 
 -->vim default
add these lines at path 

location / {
  proxy_pass http://127.0.0.1:8000;
}

location /api {
  proxy_pass http://127.0.0.1:8000/api;
}


sudo systemctl restart nginx

--> check ip (it shows react app)

cd /var/www/html/

mkdir static

---go to  mynotes folder
	--> go to builds folder 
		-->copy static folder to  var/www/html/

--->sudo cp -r * /var/www/html/

sudo systemctl restart nginx

```
```



