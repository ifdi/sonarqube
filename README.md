# SonarQube and Jenkins integration

## docker-compose file for installation of SonarQube with PostgreSQL and Jenkins
\
Set these values (for linux):
```
    sysctl -w vm.max_map_count=524288
    sysctl -w fs.file-max=131072
    ulimit -n 131072
    ulimit -u 8192
```

To set them permanently, you must update /etc/sysctl.conf to reflect these values.

\
Run the containers with: 

```
docker-compose up
```

\
Jenkins available on http://localhost:8080

SonarQube available on http://localhost:9000

\
Information about Jenkins and SonarQube integration steps: 
https://tomgregory.com/sonarqube-quality-gates-in-jenkins-build-pipeline/
