# minio
[dockerhub-badge]
Minio server Docker image. Always up-to-date! Works everywhere!

### Minio Server

[Minio][minio-home] is an OSS project offering a "high performance distributed object storage server", with fabulous features like an S3-compliant API, excellent documentation, and other great features out-of-the-box. It works on multiple platforms. However, there's currently no officially maintained Docker image compatible with architectures other than amd64.

The purpose of this Docker image is to always get the latest release version of Minio server even if this image has been created some time ago. Forget about outdated version of Minio server, just restart/recreate the container of this image, and the newest release version of Minio server will be downloaded during the start.

### How can I use this?

You can run the following command to stand up a standalone instance of Minio Server on Docker:

```docker run \
  -v path_to_data:/data \
  -p 9000:9000 \
  azinchen/minio
```

### How to setup the container?

Just follow up the official [documentation][minio-docs]

[dockerhub-badge]: https://img.shields.io/docker/pulls/azinchen/minio?style=flat-square
[dockerhub-link]: https://hub.docker.com/repository/docker/azinchen/minio
[minio-home]: https://min.io
[minio-docs]: https://docs.min.io/