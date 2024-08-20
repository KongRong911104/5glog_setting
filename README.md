## 先確保安装 Docker 和 Docker Compose
在 Ubuntu 22.04 中，首先確保已安装 Docker 和 Docker Compose：
```bash
sudo apt update
sudo apt install -y docker docker-compose
```
##  下載docker-compose.yml
```bash
git clone https://github.com/KongRong911104/5glog_setting.git
```
## cd 至該目錄  
```bash
cd ./5glog_setting
```

## 執行所需的 Docker 镜像：
```bash
sudo docker-compose up -d  
```
# Grafana
### 開啟瀏覽器  
[http://該主機(宿主)的ip:3003](<http://該主機(宿主)的ip:3003/>)  
登入  
* 帳號:admin  
* 密碼:admin  

選擇skip

點擊左側**open menu > Dashboards**  
點擊畫面中間的**5g_log**  
