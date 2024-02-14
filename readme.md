ethtool -k enp1s0 | grep tcp

ethtool -K enp1s0 tso off

curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh
sudo usermod -aG docker ${USER}

su - ${USER}

<!-- create media directories -->
mkdir -p media/{movies,shows}

<!-- create download directories -->
mkdir -p downloads/{complete,temp}

<!-- create config directories  -->
mkdir -p config/{jellyfin,radarr,sonarr,nzbget}
