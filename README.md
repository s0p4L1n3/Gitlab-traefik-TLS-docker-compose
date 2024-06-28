# Deploying Gitlab on premises with Docker Compose, behind Traefik and with Self Signed Certificate




1. Download the project
2. Generate your own cert and private key for gitlab
3. Run the container
4. Display the default admin password: `sudo docker exec -it gitlab grep 'Password:' /etc/gitlab/initial_root_password`
5. You can also change it if you prefer: `docker exec -it gitlab gitlab-rake "gitlab:password:reset[root]"`
