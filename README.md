先   
sudo docker pull kongrong25/5glog_grafana:grafana  
sudo docker pull kongrong25/5glog_grafana:grafana_mysql   

下載docker-compose.yml  
在該目錄  
sudo docker-compose up -d  
sudo docker exec -it my_grafana_mysql /bin/bash  
mysql -u root -p1235 < /docker-entrypoint-initdb.d/5g.sql  
exit  
開啟瀏覽器  
localhost:3003  
帳號:admin  
密碼:admin  
選擇skip  
左側open menu > Connections > Data sources  
點擊mysql  
往下滑找到Host URL *  
該主機(宿主)的ip:3306  
滑到底部點擊Save & test  
左側open menu > Dashboards
點擊畫面中間的5g_log  
