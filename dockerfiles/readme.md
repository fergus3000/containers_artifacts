Copy docker files to their appropriate source code dirs
Build the image for each service eg.
docker build . -t poi:latest -f .\Dockerfile_3_poi_api

having locally built an image, you have to tag it and push it to acr
-- take userprofile for example...
docker tag userprofile:latest myregistry.azurecr.io/userprofile:1.0.0
