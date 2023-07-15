## Jornada tasks -  2023-07-14

  - [] Containerize Webapps for CI/CD:
    - [ ] TOBI
      - [x] repo + container
      - [] apache/nginx accessions
      - [] CICD
    - [x] FRIDA
      - [x] repo + container
      - [] apache/nginx accessions
      - [] CICD
    - [] Climate-quick-guide (priority)
      - [] repo + container
      - [] apache/nginx accessions
      - [] CICD
    - [] transition-sandbox
    - [] WATA (priority)
      - [] repo + container
      - [] apache/nginx accessions
      - [] CICD

  - [] transfer WebApps (ubuntu 16/wsgi) to jornada-SWBAPPS(x.x.x.169)
    - dependencies: setup docker, nginx, certbot

  - [] Migrate SWClimateHub maps (resolve vulnerability)
    - [] containerize Geoserver (JVM or Tomcat)
    - [] deploy containerized geoserver on K8S(x.x.x.140)
    - [] containerize Coombs webmap and deploy on K8s
    - [] migrate webapps layers on separate PG instance on K8s

  - [] deploy minikube/micrik8s cluster on k8m(x.x.x.170), k8n1(x.x.x.171), k8n2(x.x.x.172) (low priority)
    - [] deploy using terraform (low priority)
    - [] migrate webapps from different projects and segregate by namespaces (low priority)
    - [] figure out how to make the cluster services externally available 
      - Traefik: outside of VM- ip address paradigm, how to route a service through a specific domain 

  - [] set up Graphana/prometheus monitoring
  - [] create private github action runners within jornada
  - [] create private dockerhub image registry

## LDC tasks 2023-07-14
  - [] Finish main API auth doc 
  - [] Ingest: 
    - [] DurP (tall)
    - [] postingest Durp
  - [] migrate python ingestion to Apache airflow (low priority)