#  Docker Nginx Reverse Proxy Setup

This project sets up a local reverse proxy using **Docker**, **Docker Compose**, and **Nginx**. It routes HTTP traffic to two backend services — `httpbin` and `whoami` — using both:

 **Path-based routing** (e.g. `/httpbin/`)  
 **Subdomain-based routing** (e.g. `httpbin.local.example.com`)
##  Project Structure
proxysetup/
├── docker-compose.yml
└── nginx/
└── default.conf



---
##  What It Does

This Nginx reverse proxy supports:

###  Path-Based Routing


 `http://local.example.com/httpbin/` | `httpbin` container |
 `http://local.example.com/whoami/` | `whoami` container |

### 🌐 Subdomain-Based Routing


 `http://httpbin.local.example.com/` | `httpbin` container |
 `http://whoami.local.example.com/` | `whoami` container |
 `/etc/hosts` to point `local.example.com` to your machine (`127.0.0.1`).
 ## screenshots:
   ### docker:
   ![image](https://github.com/user-attachments/assets/fab06010-f15f-4c6c-8432-159f114c7fc6)
   
 ## path based:
   ### httpbin
  ![image](https://github.com/user-attachments/assets/f19f065b-e687-4100-ac37-34f78f68f896)
   ### whoami
   ![image](https://github.com/user-attachments/assets/2c6eff3b-0df9-4d77-9403-71fb5aebc4fc)

 ## subdomain 
   ### whoami
 ![image](https://github.com/user-attachments/assets/67519f3f-8358-4130-9463-a39f5def4030)
  ### httpbin
  ![image](https://github.com/user-attachments/assets/81c0789f-7af4-45be-b7f8-9cf7f82102f2)



