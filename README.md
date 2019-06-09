# Docker + Node 12 on board. [Hub](https://hub.docker.com/r/shanhaichik/docker-node-12)

**Official image repositories:**
[Docker](https://github.com/docker-library/docker) and [Node](https://github.com/nodejs/docker-node/blob/5d8827883ba24066cec73f6d6c3e70c3ec4e1b28/12/alpine/Dockerfile).


## Usage
```yaml
job
    image: shanhaichik/docker-node-12:latest
    script:
        - npm install
        - npm run build
        - docker login 
        - docker build . -t some-image
        - docker push some-image
```