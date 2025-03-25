## Ambiente Virtual
python3 -m venv ./ambienteVirtual
source ./ambienteVirtual/bin/activate
pip install -r requirements.txt
deactivate

## Docker 
sudo sysctl -w vm.max_map_count=262144

(sudo docker-compose up -d)

sudo docker-compose -f 'docker-compose.yaml' up -d --build "setup" 

sudo docker-compose -f 'docker-compose.yaml' up -d --build "es01"

sudo docker-compose -f 'docker-compose.yaml' up -d --build "kibana"

