# Link Extractor: Step 0

A basic page scraping script that prints out all the hyper references of the given web page.

## Try it out

```bash
./linkextractor.py http://example.com/
```

## Possible difficulties

* Is the script executable? (`chmod a+x linkextractor.py`)
* Is `Python` installed on the machine?
* Can you install software on the machine?
* Is `pip` installed?
* Are `requests` and `beautifulsoup4` Python libraries installed?

## Containerize it!

**Option 1:** Create a Dockerfile
Create a file named `Dockerfile` and type or copy the following contents in to it:

```dockerfile
FROM       python:3.7-alpine
LABEL      maintainer="Jim Armstrong <@jdarmstro>"

RUN        pip install beautifulsoup4
RUN        pip install requests

WORKDIR    /app
COPY       linkextractor.py /app/
RUN        chmod a+x linkextractor.py

ENTRYPOINT ["python", "./linkextractor.py"]
```

**Option 2:** Copy the cheats file
`cp cheats/Dockerfile .`


## Build the image

`docker build . -t linkextractor:v0`


## Run the container

`docker run linkextractor:v0 https://docker.com`

You can use any URL you want above.