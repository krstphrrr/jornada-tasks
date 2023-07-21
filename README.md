## Jornada tasks -  2023-07-14

  - [ ] Containerize Webapps for CI/CD:
    - [ ] TOBI 
      - [x] repo + container
      - [ ] add secrets (to new webapps)
      - [ ] apache/nginx conf
      - [ ] CICD (unrem paralellism)
    - [ ] FRIDA 
      - [x] repo + container
      - [ ] add secrets (to new webapps)
      - [ ] apache/nginx conf
      - [ ] CICD (unrem paralellism)
    - [ ] Climate-quick-guide (priority)
      - [x] repo + container
      - [ ] apache/nginx conf
      - [ ] CICD (unrem paralellism)
    - [ ] transition-sandbox
      - [x] repo + container
      - [ ] apache/nginx conf
      - [ ] CICD (unrem paralellism)
    - [ ] WATA (priority)
      - [x] repo + container
      - [ ] apache/nginx conf
      - [ ] CICD (unrem paralellism)

  - [x] transfer WebApps (ubuntu 16/wsgi) to jornada-SWBAPPS(x.x.x.169)
    - dependencies: setup docker, nginx, certbot
    - [x] set up new limited user to run swarm
    - [x] clone locally

  - [ ] Migrate SWClimateHub maps (resolve vulnerability - High priority)
    - [x] containerize Geoserver (JVM or Tomcat)
      - commit [08f9ca0](https://github.com/krstphrrr/geoserver-port/commit/08f9ca0065755404d145be167678da8307ca27ce)
    - [x] deploy containerized geoserver on jer (x.x.x.187)
    - [ ] containerize Coombs webmap and deploy on jer
    - [x] migrate webapps layers on separate PG instance on jer

  - [ ] deploy minikube/micrik8s cluster on k8m(x.x.x.170), k8n1(x.x.x.171), k8n2(x.x.x.172) (low priority)
    - [ ] deploy using terraform (low priority)
    - [ ] migrate webapps from different projects and segregate by namespaces (low priority)
    - [ ] figure out how to make the cluster services externally available 
      - Traefik: outside of VM- ip address paradigm, how to route a cluster service through a specific domain 
      - test PG migration, replication streams and persistent volumes

  - [ ] set up Graphana/prometheus monitoring
  - [ ] create private github action runners within jornada
  - [ ] create private dockerhub image registry

## LDC tasks 2023-07-14
  - [ ] Finish main API auth doc 
  - [ ] Ingest: 
    - [ ] DurP (tall)
    - [ ] postingest Durp
  - [ ] migrate python ingestion to Apache airflow (low priority)