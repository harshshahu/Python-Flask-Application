This application is basic Python Flask Application that shows output like:
Hello from Flask App!

After git clone

install the Docker compose, use below command to download the Docker Compose:
1:
sudo mkdir -p /usr/local/lib/docker/cli-plugins
    (What it does:
    mkdir → creates a directory
    -p → creates parent directories if they don’t exist
    /usr/local/lib/docker/cli-plugins → directory where Docker looks for CLI plugins)
    
2:
sudo curl -SL https://github.com/docker/compose/releases/download/v2.27.0/docker-compose-linux-x86_64 -o /usr/local/lib/docker/cli-plugins/docker-compose
    (Downloads Docker Compose v2.27.0 and saves it as docker-compose in the plugin directory)

3:
sudo chmod +x /usr/local/lib/docker/cli-plugins/docker-compose
    (What it does:
    chmod	-> change permissions
    +x -> make executable
    path	-> docker-compose file)

4: to check docker compose version:
docker compose version

after successful installation, build the docker image, than run the docker compose by using the following command:
docker compose up -d 

how to stop docker compose?
docker compose down 
