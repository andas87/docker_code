# docker_code

This repository contains the Docker code for ecomm capstone project.
It contains -
1. Dockerfile for building image of tomcat, mysql, jdk (Dockerfile)
2. SQL scripts for mysql setup in docker image (mysqldb_conf.sh)
3. Entrypoint script used in image for starting tomcat and MySQL(entrypoint.sh)
4. Ansible playbook for setting up docker on a machine (setup_ecomm_docker.yaml)
5. Ansible playbook for deploying war file and starting the container on a remote machine (deploy_ecomm_docker.yaml)
