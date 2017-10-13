Redis Container for OpenShift 3
===============================

Version of a popular Redis Docker image (docker pull spec: redis)
that will run on OpenShift 3 with the default Security Context Constraint (SCC)
of restricted.

The redis docker image (at least version 4.0.2) runs fine under the **restricted** SCC already,
so no customization of the image is required at this time.

# Importing Docker image into OpenShift
There is a YAML file in the openshift directory (redis-imagestream.yml) which will
import the redis image(s) into the internal registry of an OpenShift
cluster.
