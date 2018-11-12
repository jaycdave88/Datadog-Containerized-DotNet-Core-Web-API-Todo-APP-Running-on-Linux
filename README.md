**Setup**
> Within the `docker-compose.yaml` - edit the key value for `DD_API_KEY` with your Datadog API Key. 

**Run**
> `docker-compose up` 

**Information on routes and payload:**
> To hit the endpoints, use a tool like [Postman](https://www.getpostman.com/apps) and use the endpoint of: `http://localhost:80/{ENDPOINTS_FOUND_BELOW}`

- **POST** /api/todo/
    - Create a new Todo item.
        - i.e.: ```{"name": "siting at the airport","isComplete": false}```
- **GET** /api/todo/
   - Will return **all** Todo items.
- **GET** /api/todo/{id}
    - Will return a specific Todo item.
- **PUT** /api/todo/{id}
    - Will update the Todo item.
        - i.e.: ```{"name": "siting at the airport","isComplete": true}```
- **DELETE** /api/todo/{id}
    - Delete a specific Todo item by giving it the ID.

