先   
sudo docker pull kongrong25/5glog_grafana:grafana  
sudo docker pull kongrong25/5glog_grafana:grafana_mysql   

下載docker-compose.yml  
在該目錄  
sudo docker-compose up -d  
開啟瀏覽器  
localhost:3003  
帳號:admin  
密碼:admin  
選擇skip  
左側open menu > Connections > Data sources  
點擊mysql  
往下滑找到Host URL *  
將localhost改成該主機(宿主)的ip  
滑到底部點擊Save & test  
左側open menu > Dashboards
點擊畫面中間的5g_log  
