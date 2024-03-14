# Shadowsocks-Rust Docker Setup

This repository contains a Docker Compose file for setting up a Shadowsocks-Rust server, an efficient and secure way to bypass internet censorship. The `docker-compose.yml` file simplifies the deployment process on any server or local machine that supports Docker.

## Prerequisites

Before starting, ensure you have Docker, Docker Compose, and Midnight Commander (mc) installed on your machine. These tools are required for setting up and managing the Shadowsocks-Rust server.

## Installation

Follow these steps to deploy your Shadowsocks-Rust server:

1. **Install Docker, Docker Compose, and Midnight Commander (mc):**

   Depending on your operating system, the installation process may vary. Please refer to the official documentation for [Docker](https://docs.docker.com/get-docker/), [Docker Compose](https://docs.docker.com/compose/install/), and Midnight Commander (install via your OS's package manager, e.g., `apt install mc` on Debian/Ubuntu).

2. **Download the `docker-compose.yml` file:**

   Clone this repository or simply download the `docker-compose.yml` file using:
   ```bash
   git clone https://github.com/ckazi/shadowsocks-rust

Configure the environment variables:

Navigate to the directory containing docker-compose.yml and open it in an editor. You must set the SS_PASSWD environment variable to a secure password. Optionally, you can change the SS_IP variable, but it's typically fine to leave it as 0.0.0.0.

Launch the server:

With the configuration set, start your Shadowsocks-Rust server by running:
docker-compose up -d

Install a Shadowsocks client:

To connect to your server, you'll need a Shadowsocks client. For Android devices, download the app from Google Play.

Configure the Shadowsocks client:

Add a new connection with the server IP address (the IP of the machine where you've deployed the server), the port, and the password you specified in the docker-compose.yml file. Use aes-256-gcm as the encryption method.

Enjoy unrestricted internet access.

Support

If you found this project helpful and wish to support further development, consider donating to the following Monero (XMR) address:

41ugNNZ5erdfj8ofHFhkb2gtwnpsB25digy6DWP1kCgRTJVbg6p7E6YMWbza7iCSMWaeuk9Qkeqzya8mCQcQDymH7P2tgZ5

Your support is greatly appreciated!
