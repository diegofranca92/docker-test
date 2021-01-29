## Instalar o Docker
 sudo apt-get install docker.io

## Reiniciar o serviço do docker
sudo systemctl restart docker

## Verificar o status do docker
sudo systemctl status docker

## Ativar no boot
sudo systemctl enable docker

## Instalar o portainer (Altere o seu diret贸rio Home)
sudo docker run -d -p 9000:9000 --name portainer --restart always -v /var/run/docker.sock:/var/run/docker.sock -v /home/juliano/Portainer/data:/data portainer/portainer

## Abra o navegador
localhost:9000
