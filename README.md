# READ ME

### Generate root password

Graylog docker container accepts SHA256 hashed root password. Generate SHA256 hash of your root password using following command.

```echo -n "password" | sha256sum```

It will generate SHA256 hashed password.

### Set environment variables

Create a `.env` file at the root of the project and set the following variables in the file

```GRAYLOG_ROOT_PASSWORD=SHA256 hashed password```

```GRAYLOG_PASSWORD=16 character super secret password```

### Run docker-compose

Run the docker-compose.

```docker-compose up -d```

### Open Graylog

Now go to the [http://localhost:9000](http://localhost:9000) to access Graylog server. Enter the following credentials to login

```username: admin```
```password: SHA256 hashed password```
