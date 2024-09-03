# TL;DR

```bash
docker compose up
```

# Dependencies

Reference the following for quick start
- `Dockerfile` for setup and how to run
- `requirements.txt` for python dependencies

Run with `python -m flask run --host=0.0.0.0 --port=8000`.

Reference Flask documentation for more controls.

# Docker

Most of the docker setup files created with `docker init`.

## Run with docker compose

`docker compose up`

Your application will be available at http://localhost:8000.

## Deploying your application to the cloud

(This is a standard walkthrough from `docker init`)

First, build your image, e.g.: `docker build -t myapp .`.
If your cloud uses a different CPU architecture than your development
machine (e.g., you are on a Mac M1 and your cloud provider is amd64),
you'll want to build the image for that platform, e.g.:
`docker build --platform=linux/amd64 -t myapp .`.

Then, push it to your registry, e.g. `docker push myregistry.com/myapp`.

Consult Docker's [getting started](https://docs.docker.com/go/get-started-sharing/)
docs for more detail on building and pushing.

# References
* [Docker's Python guide](https://docs.docker.com/language/python/)
* [Flask](https://flask.palletsprojects.com/en/3.0.x/)
* [Dungeons](https://scryfall.com/search?q=t%3Adungeon)