**PROJECT CONFIGURATION CREDENTIALS:**  
`DB_USERNAME=spring;DB_PASSWORD=spring;DB_URL=jdbc:mysql://localhost:3306/GridDB?allowPublicKeyRetrieval=true&useSSL=false`

**BEFORE USING THE BACKEND, USE THIS COMMANDS FIRST (after docker-compose file was executed):**

>  *Enter the MySQL container:*

    docker exec -it grid-mysql-container bash

> *Connect to MySQL using the command:*

    mysql -u root -pspring

  

> Next, grant privileges to the user 'spring' on the 'GridDB' database.
> Execute the following SQL query:

    GRANT ALL PRIVILEGES ON GridDB.* TO 'spring'@'%';
	FLUSH PRIVILEGES;


> *Exit MySQL and the container:*

    exit
    exit

  

**AFTER THIS EXECUTE PROJECT**
