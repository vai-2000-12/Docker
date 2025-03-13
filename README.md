# 📌 Docker Commands Cheat Sheet 🚀

This **README** contains all the essential Docker commands you learned, categorized for easy understanding! 🎉

---

## 🔹 1. Docker Basics
| Command | Description |
|---------|-------------|
| `docker run hello-world` | Runs a test container to check Docker installation. |
| `docker ps` | Lists running containers. |
| `docker ps -a` | Lists all containers (including stopped ones). |
| `docker images` | Shows all available images. |
| `docker rmi <IMAGE_ID>` | Removes a Docker image. |
| `docker rm <CONTAINER_ID>` | Removes a stopped container. |
| `docker container prune` | Removes all stopped containers. |

---

## 🔹 2. Working with Containers
| Command | Description |
|---------|-------------|
| `docker run -it ubuntu bash` | Starts an interactive Ubuntu container. |
| `docker start <CONTAINER_ID>` | Starts a stopped container. |
| `docker stop <CONTAINER_ID>` | Stops a running container. |
| `docker restart <CONTAINER_ID>` | Restarts a container. |
| `docker exec -it <CONTAINER_ID> sh` | Opens a shell inside a running container. |
| `docker logs <CONTAINER_ID>` | Displays logs of a container. |

---

## 🔹 3. Networking in Docker
| Command | Description |
|---------|-------------|
| `docker network ls` | Lists all Docker networks. |
| `docker network create my_network` | Creates a custom network. |
| `docker network inspect my_network` | Shows details of a network. |
| `docker run --network my_network --name my_container -d alpine sleep 1000` | Runs a container inside a custom network. |

---

## 🔹 4. Working with Docker Volumes
| Command | Description |
|---------|-------------|
| `docker volume ls` | Lists all Docker volumes. |
| `docker volume create my_volume` | Creates a new volume. |
| `docker volume inspect my_volume` | Shows details of a volume. |
| `docker run -d --name volume_test -v my_volume:/app busybox sleep 100` | Attaches a volume to a container. |
| `docker exec -it volume_test sh` | Enters a container to check mounted volume data. |
| `docker rm -v <CONTAINER_ID>` | Removes a container along with its volume. |
| `docker volume rm my_volume` | Deletes a Docker volume. |

---

## 🔹 5. Pulling & Managing Images
| Command | Description |
|---------|-------------|
| `docker pull ubuntu` | Downloads the Ubuntu image from Docker Hub. |
| `docker run ubuntu` | Runs an Ubuntu container. |
| `docker pull hello-world` | Pulls the Hello World image. |
| `docker run --rm hello-world` | Runs and automatically removes the container after execution. |

---

## 🔹 6. Miscellaneous Commands
| Command | Description |
|---------|-------------|
| `cat /etc/os-release` | Shows OS details inside a container. |
| `apt update` | Updates package lists inside an Ubuntu container (if network is available). |
| `exit` | Exits from a running container shell. |

---

## 🎯 Next Steps
- Practice more Docker commands 🚀
- Learn **Docker Compose** 🏗️
- Experiment with **Dockerfile & Image Building** 🛠️
- Explore **Docker Swarm & Kubernetes** ⚡

---

Happy Dockering! 🐳🎉
