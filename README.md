# PostgreSQL Docker-Compose Setup

This repository provides a pre-configured setup for running PostgreSQL with Docker Compose. It includes a Docker Compose file along with some useful scripts to facilitate easy setup and management of the PostgreSQL database.

## Prerequisites

To use this setup, you need to have Docker and Docker Compose installed on your system. If you don't have them installed, please follow the official installation guide for your operating system:

- Docker: https://docs.docker.com/get-docker/
- Docker Compose: https://docs.docker.com/compose/install/

## Quick Start

Follow these steps to quickly set up and run PostgreSQL with Docker Compose:

1. Clone this repository to your local machine:

      ```bash
      git clone https://github.com/semyonkrutolevich/psql-docker-compose-configs.git your-project-folder
      ```

2. Navigate to the repository folder:

      ```bash
      cd your-project-folder
      ```

3. Update the .env file with your desired configuration. You can modify the environment variables from .env.sample file according to your needs.

4. Update pg_hba.conf configuration to restrict or allow connections.

5. To configure the Postgres database server, you can modify the `postgresql.conf` file.

6. Start the PostgreSQL database using Docker Compose:

      ```bash
      docker-compose up -d
      ```
   
   This command will start the PostgreSQL container in the background.

7. Access the PostgreSQL database:

   - Host: localhost
   - Port: 5432
   - User: <your_username>
   - Password: <your_password>
   - Database: <your_database>

8. Access the PGAdmin databases administration and management tool at the `localhost:15433` address.

9. Enjoy using PostgreSQL! You can connect to the database using any PostgreSQL client or tool of your choice.

## Customization

This setup is pre-configured to be ready to use out of the box. However, if you need to customize the PostgreSQL configuration or make any changes, you can edit the docker-compose.yml file. Refer to the official Docker Compose documentation for more details: https://docs.docker.com/compose/compose-file/

## License

This repository is licensed under the MIT License.

## Acknowledgments

- PostgreSQL - The powerful open-source relational database management system.
- Docker - The platform for building and running containers.
- Docker Compose - The tool for defining and running multi-container Docker applications.

---
