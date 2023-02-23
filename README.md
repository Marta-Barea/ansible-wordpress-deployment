# ansible-wordpress-deployment

This is an Ansible playbook that installs and configures a WordPress site on a Linux server. It performs the following tasks:

- Installs the UFW firewall and sets up rules to allow inbound traffic on ports 80, 443 (TCP and UDP), and 22023 (TCP).
- Creates a directory for the WordPress installation.
- Downloads the latest version of WordPress and extracts it to the created directory.
- Sets ownership and permissions for the WordPress directory.
- Installs and configures Certbot for obtaining SSL certificates.
- Sets up a cron job to renew SSL certificates.
- Installs and configures the Nginx web server.
- Creates a logs directory for Nginx.
- Configures Nginx for HTTP and HTTPS traffic, with the latter using SSL certificates obtained from Certbot.
- Installs MySQL for PHP and sets up a database for WordPress.
