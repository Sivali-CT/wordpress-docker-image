# Read this!

After that, run the following command:
```bash
docker compose up -d
```
Wait until the image finishes building and the container starts running. You can check the status of the container using the command:

```bash
docker ps
```

Next, let's create the db inside mysql container:
```bash
docker exec -it local-mysql mysql -u root -p
```

```bash
mysql> create database wordpress;
```

Now open `http://localhost:8080/wp-admin/install.php` in your browser.

![wordpress and mysql in docker container](https://res.cloudinary.com/andinianst93/image/upload/v1704281437/kjigd9dpxsp5gopya73q.png)

Don't forget to:
```bash
docker compose down
```
after you finish.
