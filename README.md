# ProxiBanqueSi-Docker-config

ProxybanqueSI README

Welcome to ProxybanqueSI! This guide will help you set up and run the ProxybanqueSI Angular app and Java Spring Boot web service using Docker containers.

How to Run Apps with Docker ? :

Create Docker containers and run the apps:
```bash
docker-compose up
```
> **Caution: Important Note**
>
> Please be aware of the following:
>
>- Show processes running on port 80:
>
>```bash
>sudo netstat -tuln | grep 80
>```
>or
>
>```bash
>sudo lsof -i :80
>```
>
>- Stop a process on a port:
>```bash
>sudo kill <PID>
>```
>
>- Kill all processes of port 80:
>```bash
>sudo killall -9 -v $(sudo lsof -t -i:80)
>```
>
>or
>
>```bash
>sudo pkill -f ":80"
>```
>***
>

Useful Docker Commands:

- Show the IP address of a Docker container:
```bash
docker-compose exec angular-app hostname -i
```