## Komari - A simple server monitor tool

Komari is a lightweight self-hosted server monitoring tool designed to provide a simple and efficient server performance monitoring solution. It supports viewing server status through a web interface and collecting data through lightweight agents.

### How to Find the Administrator Password

After the application is installed, please go to the application details page of `komari-XXXXXXXX` and find **Pod List** -> **Logs**.

In the logs, you can find the initial administrator password.

```bash
2025/07/21 06:49:03 Komari Monitor 1.0.0 (hash: 88a441da232a20e3096807bc51e6dd27e5868e33)
2025/07/21 06:49:03 Using SQLite database file: /app/data/komari.db
2025/07/21 06:49:03 Info: Environment variable TZ not set, using default UTC timezone (UTC).
2025/07/21 06:49:03 Default admin account created. Username: admin , Password: cY5J7vln9B-G
2025/07/21 06:49:03 Using ip-api.com as GeoIP provider.
[GIN] 2025/07/21 - 06:49:10 | 200 |     520.476µs |    47.79.94.226 | GET      "/"
[GIN] 2025/07/21 - 06:49:12 | 200 |     486.889µs |    47.74.47.231 | GET      "/"
[GIN] 2025/07/21 - 06:49:13 | 200 |     764.485µs |    47.74.47.231 | GET      "/registerSW.js"
[GIN] 2025/07/21 - 06:49:13 | 200 |    2.209823ms |    47.74.47.231 | GET      "/assets/chunk-react-vendor-Csw2ODfV.js"
[GIN] 2025/07/21 - 06:49:13 | 200 |   13.443539ms |    47.74.47.231 | GET      "/assets/entry-index-Cs6QGJpg.js"
```

Here, `Username: admin` is the administrator account name, which is `admin`. `Password: cY5J7vln9B-G` is the administrator password, which is `cY5J7vln9B-G`.


### Notice

Protect the login address: Set access restrictions to prevent unauthorized direct access.
    
Use a complex password: Create a password that includes uppercase letters, lowercase letters, numbers, and special characters to increase cracking difficulty.
    
Avoid common usernames: Refrain from using common usernames like "admin" or "root" to reduce the risk of brute-force attacks.
    
Regularly change passwords: It is recommended to update your password periodically to mitigate security risks associated with long-term usage of the same password.
    
Enable multi-factor authentication: Adopt two-factor authentication to add an extra layer of security beyond just the password.
    
Limit login attempts: Set a maximum number of failed login attempts, and temporarily lock the account once it is exceeded to prevent brute-force attacks.
    
Configure unusual login notifications: Set up alerts for abnormal login activity to be informed and respond promptly to potential security issues.
    
Conduct regular security audits: Periodically review account security logs and system configurations to quickly identify and fix potential vulnerabilities.
        