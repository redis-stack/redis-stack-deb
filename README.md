# redis-stack-deb

This repository takes the promoted [redis-stack](https://github.com/redis-stack/redis-stack) debian archive, updates a deb repository, and uploads the artifacts to S3.

Publishing debs involves:

1. Publishing a release using the release tool in [redis-stack](https://github.com/redis-stack/redis-stack).
2. Waiting for the [publish release](https://github.com/redis-stack/redis-stack/actions/workflows/release.yml) action to complete, promoting the releases.
3. Tagging this repository, with the same tag created in redis-stack.
