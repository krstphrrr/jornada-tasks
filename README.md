
## 2024-04-05 
- Security: migrating away from docker/swarm to remove the need to have root privileges on host machines to run the docker daemon. k8s, podman, buildah
- AWS:
- - exporting cloud formation manifests
- - reviewing alternatives for the large pg instance
- reviewing options for self-hosted runners as we can't grant external access to the github runners with the new firewall setup
- review rap timeouts 
- review the k8s host machines nginx conf to enable management of wp instances 
- small node app that uses lambda (external fetcher) to report how externally accessible our sites are
- - on-premise host runs app on cron. app creates a json of website uptime. if any of these are false, shoot single email ABOUT THE FALSE service to uptime account which is forwarded from there to others. 

## 2024-04-04
- updated the nginx configuration for both rap and the ldc fastify api at the on-premise servers. These two applications leverage a containerized nginx instance to serve an angular aplication compiled to hmlt and a companion nodejs app. in both cases, misconfiguration were taking the container instances down regularly, as they were running only a single nginx replica. 

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