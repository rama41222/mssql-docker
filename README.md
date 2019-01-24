MS Sql on mac
===================

Setup
-------------

Note: Each of these steps should be performed in the root directory.

 - Create a .env `mv .env.template .env`
 - Add the suitable values
 ```
 ACCEPT_EULA=Y
 SA_PASSWORD=your password
 ``` 
## Running on Docker

| Script          | Description                                     |
| --------------- | ----------------------------------------------- |
| `docker-compose down`   | Remove all the resources created by docker compose previously                       |
| `docker-compose run --rm --service-ports mssql -d` | Run the application in background |
| `docker-compose run --rm --service-ports mssql` | Run the app in foreground |

###### More on [service ports](https://docs.docker.com/compose/reference/run/)
