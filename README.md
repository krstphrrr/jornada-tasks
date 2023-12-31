## Tasks - 2023-07-26

  - [x] disable test.jornada.nmsu.edu
  - [x] resolve jornada-k8s.nmsu.edu/wp-json vulnerability
  - [ ] remove duplicates from tall (lpi, gap, height) 


## Jornada tasks -  2023-07-14

  - [x] Containerize Webapps for CI/CD:
    - [x] TOBI 
      - [x] repo + container
      - [x] add secrets (to new webapps)
      - [x] apache/nginx conf
      - [x] CICD (unrem paralellism)
    - [x] FRIDA 
      - [x] repo + container
      - [x] add secrets (to new webapps)
      - [x] apache/nginx conf
      - [x] CICD (unrem paralellism)
    - [x] Climate-quick-guide (priority)
      - [x] repo + container
      - [x] apache/nginx conf
      - [x] CICD (unrem paralellism)
    - [ ] transition-sandbox
      - [ ] repo + container
      - [ ] apache/nginx conf
      - [ ] CICD (unrem paralellism)
    - [x] WATA (priority)
      - [x] repo + container
      - [x] apache/nginx conf
      - [x] CICD (unrem paralellism)

  - [x] transfer WebApps (ubuntu 16/wsgi) to jornada-SWBAPPS(x.x.x.169)
    - dependencies: setup docker, nginx, certbot
    - [x] set up new limited user to run swarm
    - [x] clone locally

  - [x] Migrate SWClimateHub/asombro maps (resolve vulnerability - High priority)
    - [x] containerize Geoserver (JVM or Tomcat)
      - commit [08f9ca0](https://github.com/krstphrrr/geoserver-port/commit/08f9ca0065755404d145be167678da8307ca27ce)
    - [x] deploy containerized geoserver on jer (x.x.x.187)
    - [x] containerize Coombs webmap and deploy on jer
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
  - [x] Ingest: 
    - [x] DurP (tall)
    - [x] postingest Durp
  - [ ] migrate python ingestion to Apache airflow (low priority)