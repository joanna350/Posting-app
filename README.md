#### Evironment
- Python3
- Mac OS Catalina / Ubuntu 18.04

#### Project/App Setup
- Setup directory
```
mkdir __folder_name__ && cd $_

python3 -m venv .
source bin/activate
pip3 install -r requirements.txt
```

#### React Frontend
- Install Node
```
(Mac) brew install node
```
(Ubuntu) [steps](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-18-04)

- under the directory [frontend]
```
npm init -y
npm i webpack webpack-cli --save-dev
npm i @babel/core babel-loader @babel/preset-env @babel/preset-react --save-dev
npm i react react-dom --save-dev
npm run dev
```

#### Run
- At the root of the project
```
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py runserver
```

#### Create Test Data
- Add data under the endpoint ```localhost:port/api/lead/```


#### Scheduler
```
python3 scheduler.py '2011-02-15' '2021-08-31' 11 7 15 18
```
- Format to pass start of the period, end of the period, day to post, days to comment as parameters
