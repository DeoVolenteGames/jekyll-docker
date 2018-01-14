# DVG Docker

An extension of the official [Jekyll Docker image][jekyll-image] with Python and
the [AWS Command Line Interface][awscli] so that it's possible to push build
artifacts to S3. It also supports git-lfs and gzip.

## How to use

1. Build dockerfile in docker directory:
    ```sh
    docker build -t deovolentegames/jekyll .
    ```
1. Login to server (`docker login`), then push the latest image
    ```sh
    docker push deovolentegames/jekyll:latest
    ```

See [the offical docs][docker-docs-share] for more info

## Todo

1. Add ability build Docker images automatically using Docker CI and Github?

[jekyll-image]: https://hub.docker.com/r/jekyll/jekyll/
[awscli]: https://aws.amazon.com/cli/
[docker-docs-share]: https://docs.docker.com/get-started/part2/#share-your-image
