**PROJECT CONFIGURATION CREDENTIALS:**  
For localhost:
`DB_USERNAME=spring;DB_PASSWORD=spring;DB_URL=jdbc:mysql://localhost:3306/GridDB?allowPublicKeyRetrieval=true&useSSL=false`

**Deprecated section, no need to use it anymore**
>  *Enter the MySQL container:*

    docker exec -it grid-mysql bash

> *Connect to MySQL using the command:*

    mysql -u root -pspring

  

> Next, grant privileges to the user 'spring' on the 'GridDB' database.
> Execute the following SQL query:

    GRANT ALL PRIVILEGES ON GridDB.* TO 'spring'@'%';
	FLUSH PRIVILEGES;


> *Exit MySQL and the container:*

    exit
    exit

  

**After This Execute Project**
