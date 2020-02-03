## 2001.dev (Unrelease)

NOTES:

UPGRADE NOTES:

ENHANCEMENTS:
* Rover login argument changes to rover login [tenant] [subscription]
* Deleting previous terraform.tfstate from rover after each execution
* terraform version to 0.12.20
* az cli version to 2.0.80
* git version to 2.25.0
* require sudo to execute docker in docker to access host docker deamon
* Adding bzip2
* Refactoring the Dockerfile to support multi-stage build and reduce sub-sequent rebuild

BUG FIXES:
* change *.sh from CRLF to LF
* moving docker-compose to /usr/bin
* fixing a curl for jq in the Dockerfile

NEW FEATURES:

# v1912.1312
UPGRADE NOTES:
* cleanup your vscode Dev Container volumes 
docker volume rm -f $(docker volume ls -f label=caf)

ENHANCEMENTS:
* non-root support - requires vscode 1.41+

# v1912.1201

UPGRADE NOTES:
* terraform version to 0.12.18

ENHANCEMENTS:
* Removing terraform.tfstate from ~/.terrafom.cache after each terraform apply
* Aligning docker tags to git tags
* Renaming install.sh by build_image.sh

BUG FIXES:
* adding vscode user to docker group