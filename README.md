# Django_API
Created a simple REST API using DRF( Django Rest Framework ) to perform CRUD operations.

Ways to Access the API:
- **Using request module in python** 

*Enter this code in jupyter notebook*
```
#POST Request 
import requests 

API_ENDPOINT = "http://127.0.0.1:8000/api/articles/"

data = {
        'article':{
        "title": "Django28",
        "description": "Framework used for Backend Development",
        "body": "Random Text",
        "author_id": 1
        }}
r = requests.post(url = API_ENDPOINT, json = data) 

#GET Request

URL = "http://127.0.0.1:8000/api/articles/"
r = requests.get(url = URL) 

data = r.json() 

print(data)
```  
