# Link Extractor: Step 3

**Note:** In this workshop we do not use Step 3 because in Step 2 we go through the process of manually making the changes shown below. Basically, at the end of Step 2 in the workshop the result is functionally equivalent to Step 3.

## Changes from the previous step

* Added a server script that uses the link extraction module written in the last step
* Server is accessible as a WEB API at `http://<hostname>[:<prt>]/api/<url>`
* Dependencies are moved to the `requirements.txt` file
* Needs port mapping to make the service accessible

## Try it out

```
$ docker image build -t linkextractor:step3 .
$ docker container run -it --rm -p 5000:5000 linkextractor:step3
```

Open http://localhost:5000/api/http://odu.edu/ in a web browser or cURL from another terminal.

```
$ curl -i http://localhost:5000/api/http://example.com/
```

Press `Ctrl + C` to terminate the service.
