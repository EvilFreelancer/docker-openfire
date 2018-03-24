# Docker Openfile skeleton

This composition contain PostgreSQL, SQL Adminer and Openfire of course.

## Okay, let's go

For fisrt you need clone and prepare the composition:

```bash
git clone https://github.com/EvilFreelancer/docker-openfire.git
cd docker-openfire
cp docker-compose.yml.dist docker-compose.yml
```

In `docker-compose.yml` you can configure any parameters what you need.
After you done you can run container by following command:

```bash
docker-compose up -d
```

And need wait some time, until system is not complete initialization
(around 5-10 minutes after first start and less than 5 minutes in any
other).

## How to update GitLab container

```bash
docker-compose pull     # Download new image of GitLab from Docker hub
docker-compose up -d    # Restart container
```

## Small how to about docker-compose

```bash
docker-compose up -d    # (re)start container, download images if not exist
docker-compose stop     # stop container
docker-compose restart  # restart container, but using the previous configuration
```

# Links

* [Openfire image in Docker](https://hub.docker.com/r/gizmotronic/openfire/)
