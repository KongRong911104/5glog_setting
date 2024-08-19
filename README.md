## 先確保安装 Docker 和 Docker Compose
在 Ubuntu 22.04 中，首先確保已安装 Docker 和 Docker Compose：
```bash
sudo apt update
sudo apt install -y docker docker-compose
```
##  下載docker-compose.yml

## cd 至該目錄  

## 使用以下命令pull所需的 Docker 镜像：
```bash
sudo docker pull kongrong25/5glog_grafana:grafana  
sudo docker pull kongrong25/5glog_grafana:mysql_grafana  
sudo docker-compose up -d  
```
# Grafana
## 開啟瀏覽器  
[http://該主機(宿主)的ip:3003](<http://該主機(宿主)的ip:3003/>)
* 帳號:admin  
* 密碼:admin

選擇skip  
左側**open menu > Connections > Data sources**  
點擊**mysql**  
往下滑找到Host URL *  
修改為  
**該主機(宿主)的ip:3306**  

滑到底部點擊**Save & test**  
**若出現錯誤**
```bash  
sudo docker exec -it my_grafana_mysql /bin/bash  
mysql -u root -p1235 < /docker-entrypoint-initdb.d/5g.sql  
exit
```  
點擊左側**open menu > Dashboards**  
點擊畫面中間的**5g_log**  
