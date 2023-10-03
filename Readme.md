```
sudo docker build -t  olelarsen/elastic-setup ./.docker/build/setup/. --build-arg VERSION_STACK=8.10.2
sudo docker build -t olelarsen/elasticsearch ./.docker/build/elasticsearch/. --build-arg ELASTIC_PORT=9200
sudo docker build -t olelarsen/kibana ./.docker/build/kibana/. --build-arg KIBANA_PORT=9200 --build-arg VERSION_STACK=8.10.2