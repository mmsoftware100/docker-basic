# Nginx on Ubuntu

```bash
# Build Image
docker build -t hello-nginx .
# Run Image
docker run -p 8080:80 hello-nginx
```


## Logs

```bash
msd@MSDs-Mac-mini-3 1-docker-hello-world % docker build -t hello-nginx .
[+] Building 0.0s (6/6) FINISHED                           docker:desktop-linux
 => [internal] load build definition from Dockerfile                       0.0s
 => => transferring dockerfile: 212B                                       0.0s
 => [internal] load metadata for docker.io/library/ubuntu:latest           0.0s
 => [internal] load .dockerignore                                          0.0s
 => => transferring context: 2B                                            0.0s
 => [1/2] FROM docker.io/library/ubuntu:latest                             0.0s
 => CACHED [2/2] RUN apt-get update &&     apt-get install nginx -y &&     0.0s
 => exporting to image                                                     0.0s
 => => exporting layers                                                    0.0s
 => => writing image sha256:e2fbdbf17410ed610566662fc37414a82537218a264a0  0.0s
 => => naming to docker.io/library/hello-nginx                             0.0s

View build details: docker-desktop://dashboard/build/desktop-linux/desktop-linux/vxgefhc9rnwyvh7q0vlkhbc4z

What's next:
    View a summary of image vulnerabilities and recommendations → docker scout quickview 
msd@MSDs-Mac-mini-3 1-docker-hello-world % 

```