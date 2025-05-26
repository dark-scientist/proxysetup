#  Docker Nginx Reverse Proxy Setup

This project demonstrates how to use **Docker** and **Docker Compose** to set up an **Nginx reverse proxy** that routes local requests to two backend services:

- `httpbin` → accessed at `/httpbin/`
- `whoami` → accessed at `/whoami/`

Everything is routed through a custom local domain: `http://local.example.com`.

##  Project Structure
proxysetup/
├── docker-compose.yml
└── nginx/
└── default.conf



---

##  How It Works

Nginx acts as a **reverse proxy**, checking the path in the URL:

- `/httpbin/` → forwarded to the httpbin container
- `/whoami/` → forwarded to the whoami container

 `/etc/hosts` to point `local.example.com` to your machine (`127.0.0.1`).
 ## screenshots:
   ### docker:
   ![image](https://github.com/user-attachments/assets/fab06010-f15f-4c6c-8432-159f114c7fc6)
 
   ### httpbin
  ![image](https://github.com/user-attachments/assets/f19f065b-e687-4100-ac37-34f78f68f896)
   ### whoami
   ![image](https://github.com/user-attachments/assets/2c6eff3b-0df9-4d77-9403-71fb5aebc4fc)


