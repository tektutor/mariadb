# Rootless Mariadb container image for Kubernetes &amp; Openshift

Supporting the OpenShift Community with Rootless Mariadb Image.

The open-source ecosystem thrives on choice and transparency. With Bitnami silently discontinuing their rootless Mariadb image on Docker Hub, many OpenShift users were left without a trusted, non-root alternative.

We provide a fully maintained rootless Mariadb container image, ready for OpenShift and other non-root environments, helping developers continue building secure and compliant containerized applications.

## Deploying this rootless mariadb in Openshift
```
oc new-app tektutor/mariadb:1.0 \
  -e MYSQL_DATABASE=wordpress \
  -e MYSQL_USER=wordpress \
  -e MYSQL_PASSWORD=wordpress \
  -e MYSQL_ROOT_PASSWORD=changeme
```
