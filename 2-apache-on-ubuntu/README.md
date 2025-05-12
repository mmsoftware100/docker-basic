# Apache on ubunut

```bash
# Build Image
docker build -t hello-apache .
# Run Image
docker run -p 8080:80 hello-apache
```

## Logs

```bash
msd@MSDs-Mac-mini-3 docker-basic % cd 2-apache-on-ubuntu 
msd@MSDs-Mac-mini-3 2-apache-on-ubuntu % docker build -t hello-apache .
[+] Building 87.5s (7/7) FINISHED                                                                               docker:desktop-linux
 => [internal] load build definition from Dockerfile                                                                            0.0s
 => => transferring dockerfile: 339B                                                                                            0.0s
 => [internal] load metadata for docker.io/library/ubuntu:latest                                                                0.0s
 => [internal] load .dockerignore                                                                                               0.0s
 => => transferring context: 2B                                                                                                 0.0s
 => CACHED [1/3] FROM docker.io/library/ubuntu:latest                                                                           0.0s
 => [2/3] WORKDIR /usr/local/apache2                                                                                            0.0s
 => [3/3] RUN apt-get update && apt-get install -y apache2 apache2-utils                                                       87.1s
 => exporting to image                                                                                                          0.4s 
 => => exporting layers                                                                                                         0.4s 
 => => writing image sha256:802f2d045fc90049ebb398de1ad37ad680625baa95e76507f8ed6364b80653d3                                    0.0s 
 => => naming to docker.io/library/hello-apache                                                                                 0.0s 
                                                                                                                                     
View build details: docker-desktop://dashboard/build/desktop-linux/desktop-linux/x6r1m469zpjvkj04nkogkjmvg                           

What's next:
    View a summary of image vulnerabilities and recommendations → docker scout quickview 
msd@MSDs-Mac-mini-3 2-apache-on-ubuntu % 
```