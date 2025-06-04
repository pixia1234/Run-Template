## Palworld Server Template

The **Palworld Server Template** is a streamlined and customizable solution designed to simplify the setup, configuration, and management of Palworld servers. This project provides a robust framework for launching and maintaining Palworld servers with minimal effort, making it ideal for both beginners and experienced server administrators. By leveraging this template, users can ensure a consistent and efficient server environment while focusing on gameplay and community building.


### Features

**Easy Setup**: Quickly deploy a Palworld server with minimal configuration.
**Customizable**: Adjust server settings such as admin password, server name, and server password to suit your needs.
**Network Configuration**: Simplified instructions for enabling internet access and mapping ports.
**Scalable**: Suitable for small private servers or larger community-based environments.
**Documentation**: Comprehensive guide to help you get started and troubleshoot common issues.


### Getting Started

Follow these steps to set up and launch your Palworld server:

### 1. Configure Environment Variables

Before deploying the server, set the following environment variables to customize your server:

**ADMIN_PASSWORD**: Set a secure password for admin access to the server.
**SERVER_NAME**: (Optional) Define a unique name for your server that will be visible to players.
**SERVER_PASSWORD**: (Optional) Set a password to restrict access to your server.

Then Deploy the Palworld Server.

### 2. Configure Network Access
To allow players to connect to your server, enable internet access for the required ports:

Go to App Launchpad:
Locate your deployed Palworld server instance (e.g., palworld-{xxxxx}) and click Details.

Manage Network Settings:
Navigate to Manage Network.
Enable internet access for the following ports:
8211: Used for game traffic.
27015: Used for Steam-related communication.

Update Configuration:
After enabling the ports, you will get 2 public addresses (e.g., xxxx.us-east-1.clawcloudrun.com), then click Update to apply the changes.

### 3. Verify Port Mapping
To find the public address and port mappings for your server:
Go to App Store => My Apps:
Scroll to the bottom of the page to view the port mapping details.

### 4. Use Public Address:
Use the provided public address and port (e.g., Public_Address:Port) to connect to your server from the Palworld client.
