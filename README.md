# DevOps NGINX Demo

A simple hands-on DevOps project that installs NGINX on Linux and serves a custom static web page.

This repository was created as a learning exercise to practice Linux administration, shell scripting, NGINX installation, Git workflows, and basic web deployment.

---

## What This Project Demonstrates

- Installing NGINX on Linux
- Managing services with `systemctl`
- Automating installation using a shell script
- Serving a custom HTML page
- Practicing Git branches and pull requests
- Basic DevOps workflow

---

## Project Structure

```text
.
├── index.html
├── install_nginx.sh
└── README.md
```

---

## Manual Installation

Update package metadata:

```bash
sudo apt-get update
```

Install NGINX:

```bash
sudo apt-get install -y nginx
```

Start the service:

```bash
sudo systemctl start nginx
```

Enable NGINX at boot:

```bash
sudo systemctl enable nginx
```

Check the service:

```bash
sudo systemctl status nginx
```

---

## Automated Installation

The repository includes:

```text
install_nginx.sh
```

Make the script executable:

```bash
chmod +x install_nginx.sh
```

Run it:

```bash
./install_nginx.sh
```

---

## Demo Web Page

The included `index.html` file can be copied to the NGINX web root:

```bash
sudo cp index.html /var/www/html/index.html
```

Then open the server IP address in a browser:

```text
http://SERVER_IP
```

---

## Technologies

- Linux
- NGINX
- Bash
- HTML
- Git
- GitHub

---

## Learning Purpose

This repository is a small DevOps learning project focused on Linux, shell scripting, NGINX, and Git workflow practice.

For my production-focused AWS automation work, see:

**SLIMTA Inventory Automation Platform**

https://github.com/Akbar324/slimta-inventory-showcase