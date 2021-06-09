# docker_code

This repository contains the Docker code for ecomm capstone project.
This includes both local and remote machine setup and deployment code.

It contains -
1. Dockerfile for building image of tomcat, mysql, jdk (Dockerfile)
2. SQL scripts for mysql setup in docker image (mysqldb_conf.sh)
3. Entrypoint script used in image for starting tomcat and MySQL(entrypoint.sh)
4. Ansible playbook for setting up docker on a machine (setup_ecomm_docker.yaml)
5. Ansible playbook for ctreating MySQL-Tomcat image for deploying ecomm (setup_ecomm_image.yaml)
6. Ansible playbook for deploying war file and starting the container on a local machine (deploy_ecomm_docker.yaml)
7. Ansible playbook for deploying war file and container on remote machine (deploy_ecomm_docker_remote.yaml)
8. Ansible playbook for deploying war file and starting the swarm on a local machine (deploy_ecomm_dockerswarm.yaml)
9. Ansible playbook for deploying war file and swarm on remote machine (deploy_ecomm_dockerswarm_remote.yaml)

Local setup
1. Create the image from Dockerfile and scripts
2. Use deploy_ecomm_docker.yaml file to create container from jenkins
3. Use deploy_ecomm_dockerswarm.yaml file to create swarm from jenkins

Remote setup
1. Run setup_ecomm_docker.yaml to install docker on remote machine
2. Run setup_ecomm_image.yaml to build image on remote machine.
3. Use deploy_ecomm_docker_remote.yaml file to create container from jenkins
4. Use deploy_ecomm_dockerswarm_remote.yaml file to create swarm from jenkins
