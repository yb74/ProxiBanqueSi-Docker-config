# ProxiBanqueSi-Docker-config

ProxybanqueSI README

Welcome to ProxybanqueSI! This guide will help you set up and run the ProxybanqueSI Angular app and Java Spring Boot web service using Docker containers.

Steps to Run Apps with Docker:

1) Build the Angular app image with:
```bash
docker build -t proxibanque-angular:latest
```

2) Build the Java Spring Boot web service image with:
```bash
docker build -t proxibanque-spring-boot:latest
```

3) Create Docker containers to run the apps:
```bash
docker-compose up
```

Useful Docker Commands:

- Show the IP address of a Docker container:
```bash
docker-compose exec angular-app hostname -i
```

- Show processes running on port 80:

```bash
sudo netstat -tuln | grep 80
```

or

```bash
sudo lsof -i :80
```

- Stop a process on a port:
```bash
sudo kill <PID>
```

- Kill all processes of port 80:
```bash
sudo killall -9 -v $(sudo lsof -t -i:80)
```

or

```bash
sudo pkill -f ":80"
```
