# docker-lnmp
## 目录结构
    -app     #站点目录
    -data    #数据目录
    -logs    #日志目录
        --mysql   #chown -R 999 mysql ,更改所有者
        --nginx
        --php-fpm
	--redis
    -server  #lnmp配置目录
        --mysql
	    --conf.d  
		my.cnf  #配置文件
	    --scripts   #备份操作
		crontabfile   #定时任务 
		mysql-backup.sh   #备份
		Dcokerfile
	    --nginx
		--certs    #证书
		--conf.d
		    default.conf  #站点配置
		Dockerfile 
		nginx.conf   #配置文件

	    --php
		Dockerfile
		php-dev.ini
		php-fpm.conf
        --redis
		Dockerfile
	docker-compose.yml

