先   
docker pull kongrong25/5glog_grafana:grafana  
docker pull kongrong25/5glog_grafana:grafana_mysql  
docker run -d --name my_grafana -p 3003:3000 kongrong25/5glog_grafana:grafana  
docker run -d --name my_grafana_mysql -p 3309:3306 kongrong25/5glog_grafana:grafana_mysql  

下載docker-compose.yml  
