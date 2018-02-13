![Apache NiFi Registry logo](https://nifi.apache.org/assets/images/registry-logo.png "Apache NiFi Registry")
# Apache NiFi Registry for Docker
## Version 0.1.0

Provides a Dockerfile and associated scripts for configuring an instance of [Apache NiFi Registry](https://nifi.apache.org/registry.html).

## Sample Usage:

From your checkout directory:

1. Build the image

        VERSION=0.1.0
        cd ${VERSION}
        docker build --build-arg VERSION=${VERSION} -t nifi-registry:${VERSION} .
		
2. Run the image

        VERSION=0.1.0
        docker run --rm -p 18080:18080 nifi-registry:${VERSION}
