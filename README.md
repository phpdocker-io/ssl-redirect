# SSL Redirect

This docker container will redirect any traffic coming on to it from HTTP to HTTPS.

## How to use:

  * Deploy
  * Make public as front controller for your sites in HTTP only

## Whyyyyy
I made this little container to get around Kong's inability to upgrade HTTP connections to HTTPS - there are third party plugins for this, but since I run Kong in Kubernetes there's no easy way to add these plugins without needing to re-build the containers and publish them to a container registry.
