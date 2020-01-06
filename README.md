Weekly Builds of Balena CLI docker image, intended to be used in CI/CD operations.

Tags:

- abferm/balena-cli:latest

Versions information :
- alpine:3.9
- balena-cli@11.0.6+

Recommended usage :

    docker run --rm -e BALENA_AUTH_TOKEN -e BALENA_APP -w /work -v /var/run/docker.sock:/var/run/docker.sock -v $(pwd):/work abferm/balena-cli:latest /bin/sh -c "balena login -t ${BALENA_AUTH_TOKEN} && balena deploy ${BALENA_APP} --build"
