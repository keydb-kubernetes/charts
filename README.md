# KeyDB charts with Flash
Kubernetes charts for KeyDB.
Copied from: https://github.com/Enapter/charts

Added features from the original repository: 
- possibility to use flash (https://docs.keydb.dev/docs/flash). It needs to use an unofficial docker build that you can find here: [dockerhub repository](https://hub.docker.com/r/renaudjester/keydb-flash), then modify your values.yaml with `imageRepository: renaudjester/keydb-flash` and `imageTag: 6.3.3`.
- new docker image has been built by adding `ENABLE_FLASH=yes` in the docker image file (`make -j$(nproc) BUILD_TLS=yes ENABLE_FLASH=yes;`) of KeyDB's repo.

