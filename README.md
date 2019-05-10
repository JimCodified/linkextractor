# Link Extractor

Link Extractor app scrapes links from a given web page.
This repository illustrates step by step approach to learn [Docker](https://www.docker.com/).

This version of the workshop is designed to be used with [Docker Desktop Community](https://www.docker.com/products/docker-desktop) but should work just about anywhere you can install or run a [Docker Engine](https://www.docker.com/products/container-runtime), including [Play With Docker](https://labs.play-with-docker.com).

It starts from running a very basic Python script and gradually leads to a multi-service container orchestration (AKA micro-service architecture).

**No Python skills required**
This workshop uses a Python example but no Python expertise is assumed or required. Step 6 switches to Ruby, but again, no Ruby knowledge is required.

## How to Use the Repository

There are multiple folders in this repo which correspond to steps in the workshop. These folders also correspond to git branches to make it easier to step through the workshop without getting lost in the folder structure. 

Here's how the recommended way to run through the workshop:

1. Install Docker Desktop Community for [Windows](https://hub.docker.com/editions/community/docker-ce-desktop-windows) or [Mac](https://hub.docker.com/editions/community/docker-ce-desktop-mac)
   * If you cannot install Docker Desktop you can also use [Play With Docker](https://labs.play-with-docker.com) or if you have a Linux machine you can install and use [Docker Engine](https://hub.docker.com/search?q=&type=edition&offering=community).
   * Run `docker version` to verify you're up and running. You should get an output something like the following:

```bash
Client: Docker Engine - Enterprise
 Version:           19.03.0-beta2
 API version:       1.40
 Go version:        go1.12.4
 Git commit:        2eed7e3
 Built:             Fri Apr 19 00:32:16 2019
 OS/Arch:           darwin/amd64
 Experimental:      false

Server: Docker Engine - Enterprise
 Engine:
  Version:          19.03.0-beta2
  API version:      1.40 (minimum version 1.12)
  Go version:       go1.12.4
  Git commit:       2eed7e3
  Built:            Fri Apr 19 00:32:21 2019
  OS/Arch:          linux/amd64
  Experimental:     false
 containerd:
  Version:          v1.2.6
  GitCommit:        894b81a4b802e4eb2a91d1ce216b8817763c29fb
 runc:
  Version:          1.0.0-rc7+dev
  GitCommit:        029124da7af7360afa781a0234d1b083550f797c
 docker-init:
  Version:          0.18.0
  GitCommit:        fec3683
```

2. Run `git checkout demo` first to setup the repos
3. Next run `git checkout step0` to start the workshop.
4. Proceed through the workshop steps (step0, step2, and step4). If you're _not_ in an instructor-led workshop the README.md will guide you through the steps.
**Note:** Not all steps are used in this workshop. We skip step1 and step3 in the class and we do not cover step5 and step6, but they all remain here as bonus steps.

## References

* The original version of this workshop was created by [Sawood Alam](https://twitter.com/ibnesayeed) and is available on [Play With Docker](https://training.play-with-docker.com/microservice-orchestration/).
   * [Original repo](https://github.com/ibnesayeed/linkextractor) 
