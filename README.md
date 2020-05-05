# Apache Reverse Proxy for Jenkins
Reverse Proxy configuration with HTTPS for **Jenkins**, **Sonarqube** and **Nexus**. Based on RHEL 7 Apache config.

This repo contains the configuration files of RHEL 7 Apache available in /etc/httpd. They have been modified in order to set up Apache as reverse proxy for:

| Tool      |                                      URL |
| :-------- | ---------------------------------------: |
| Jenkins   |  https://<myserver.mydomain.com>/jenkins |
| SonarQube |    https://<myserver.mydomain.com>/sonar |
| Nexus 3   |    https://<myserver.mydomain.com>/nexus |
| Pgadmin4  | https://<myserver.mydomain.com>/pgadmin4 |

All the above tools were deployed in the same linux box as a simple but complete CI/CD toolchain. **PostgreSQL** was also deployed locally since it was required by **SonarQube**, being this is the reason why **Pgadmin4** was also setup locally. None of them were deployed as containers, instead traditional installations were applied to make sure the outcome was simple and easy to manage by a small development team.


