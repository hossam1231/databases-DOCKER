# MySQL Dockerfile

This Dockerfile facilitates the setup of a MySQL container with port 3306 exposed. It utilizes the official MySQL base image and offers flexibility through customizable environment variables for configuration.

## Usage

### Build the Docker Image

```bash
docker build -t my-mysql-image .
```

### Run the MySQL Container

```bash
docker run -p 3306:3306 --name my-mysql-container -d my-mysql-image
```

Adjust the following environment variables as needed:

- `MYSQL_ROOT_PASSWORD`: Set the root password for MySQL.
- `MYSQL_DATABASE`: Specify the initial database to be created.
- `MYSQL_USER`: Create a MySQL user.
- `MYSQL_PASSWORD`: Set the password for the MySQL user.

### Check Container Status

To verify if the MySQL container is running, use:

```bash
docker ps
```

For a comprehensive overview, including stopped containers, use:

```bash
docker ps -a
```

### Inspect Container Details

For in-depth information on a specific container, replace `<container_name_or_id>` with the actual name or ID:

```bash
docker inspect <container_name_or_id>
```

This command provides a detailed breakdown of the container, including its current state.

Customize configurations and parameters to align with your specific use case and requirements.