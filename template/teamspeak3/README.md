# TeamSpeak Server Template

TeamSpeak is a professional voice communication platform that provides crystal-clear voice quality, military-grade security, and low latency communication perfect for gaming communities, business meetings, and online gatherings. This template makes it easy to deploy your own private TeamSpeak server with just a few clicks.

## Key Features

**Crystal Clear Voice Quality**: Experience high-quality audio with advanced codec support including Opus for exceptional clarity

**Military-Grade Security**: End-to-end encryption ensures your conversations remain private and secure

**Low Latency Communication**: Optimized for real-time communication with minimal delay

**Scalable Performance**: Supports thousands of concurrent users with efficient resource utilization

**Advanced Permission System**: Granular control over user permissions and channel access

**File Transfer Support**: Share files directly through the TeamSpeak client (when enabled)

**Server Query Interface**: Programmatic access for server administration and integration (when enabled)

**Persistent Data Storage**: All server data, settings, and configurations are preserved across restarts

**Easy Management**: Simple deployment with automatic license acceptance and credential generation

## Quick Start Guide

### 1. Deploy the Server

**Choose Your Configuration**: 

Enable **Server Query Port** if you need programmatic access for bots or administration tools

Enable **File Transfer Port** if you want users to share files through TeamSpeak

Leave both disabled for a basic voice-only server

**Click Deploy App**: The server will automatically start with a free TeamSpeak license

### 2. Get Your Admin Credentials

**IMPORTANT**: After deployment, you MUST check the container logs to get your admin credentials:

Go to your deployed app and click **Logs**

Look for these important sections:

   **Server Admin Account** (for Server Query):

   ```

                            I M P O R T A N T

                    Server Query Admin Account created

            loginname= "serveradmin", password= "YOUR_PASSWORD"

            apikey= "YOUR_API_KEY"

   ```

   **Server Admin Token** (for TeamSpeak client):

   ```

   ServerAdmin privilege key created, please use the line below

   token=YOUR_ADMIN_TOKEN_HERE

   ```

**Save these credentials** - you'll need them to manage your server!

### 3. Connect to Your Server

**Get Your Server Address**:

Go to **App Launchpad** → Find your TeamSpeak server → **Overview**

Navigate to **Network**

Note the public address for the voice port (UDP 9987)

**Connect with TeamSpeak Client**:

Download TeamSpeak client from [teamspeak.com](https://teamspeak.com/)

Use **Connections** → **Connect**

Enter your server address and port

Use the **Server Admin Token** from the logs to get admin privileges

## Configuration Options

| Option | Description | Default |

|--------|-------------|---------|

| **Enable Server Query Port** | Enables TCP port 10011 for programmatic access | Disabled |

| **Enable File Transfer Port** | Enables TCP port 30033 for file sharing | Disabled |

## Port Information

**Voice Communication**: UDP 9987 (always enabled)

**Server Query**: TCP 10011 (optional)

**File Transfer**: TCP 30033 (optional)

## Storage & Persistence

**Data Location**: `/var/ts3server/` (2GB persistent volume)

**Stored Data**: Server configuration, user data, channels, permissions

**Backup**: Data persists across server restarts and updates

## Licensing

**Free License**: Automatically accepted for up to 32 simultaneous users

**Licensed Server**: For larger deployments, place your `licensekey.dat` file in the persistent volume

**Commercial Use**: Check TeamSpeak licensing terms for commercial deployments

*TeamSpeak 3 is a trademark of TeamSpeak Systems GmbH. This template uses the official TeamSpeak Docker image and complies with their licensing terms.*