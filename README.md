# Docker bitcoin

Dockerfile of the public image [synonymdev/docker-lnd:latest](https://github.com/orgs/synonymdev/packages/container/package/lnd)


Pull the image:

```bash
$ docker pull synonymsoft/lnd:latest
```

Run the image:

```bash
$ docker run -v path/to/lnddir/:/root/.lnd -d synonymsoft/lnd:latest
```


## Release

To tag a new image with a new version:

1) Create a new folder with `VERSION` as directory name
2) Modify the GH Action in `.github/workflows/docker-publish.yml` changing the ARG `VERSION` with new created folder
3) Push in master
