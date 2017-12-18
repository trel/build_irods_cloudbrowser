# build_irods_cloudbrowser

Build the .war in a docker container
```
docker build -t build_cb:latest Dockerfile
```

Copy the .war to your host
```
docker run -it -v $(pwd):/shared_with_host build_cb:latest cp /irods-cloud-browser/irods-cloud-backend/irods-cloud-backend.war /shared_with_host/
```

[Now the .war file is ready to be deployed](https://github.com/DICE-UNC/irods-cloud-browser/blob/master/Docs/Docker.md).
