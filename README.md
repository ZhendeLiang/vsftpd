# vsftpd
docker run -d -v /var/xs/ftp:/home/vsftpd 
-p 20:20 -p 21:21 -p 21100-21110:21100-21110 
-e FTP_USER=zjmcc2 -e FTP_PASS=123 
-e PASV_ADDRESS=192.168.2.129 -e PASV_MIN_PORT=21100 -e PASV_MAX_PORT=21110 
--name vsftpd --restart=always fauria/vsftpd
