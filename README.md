
  
#apt update

#apt install npm -y

#useradd -m -s /bin/bash app
        
#cd /home/app/

#git clone https://github.com/zelar-soft-todoapp/todo.git

#cd todo/

#npm install

#vim /etc/systemd/system/todo.service

#systemctl daemon-reload
  
#systemctl start todo.service

#systemctl enable todo.service
   
#systemctl status todo.service


---------------systemd files ===  todo.service files----------------------

[Unit]
Description=Todo Service

[Service]
Environment=REDIS_HOST=172.31.91.107
ExecStart=/bin/node /home/app/todo/server.js
SyslogIdentifier =todo

[Install]
WantedBy=multi-user.target


![WhatsApp Image 2021-05-01 at 5 12 56 PM](https://user-images.githubusercontent.com/82637289/116854104-b0162080-abe6-11eb-8461-4360c6f665f5.jpeg)

![WhatsApp Image 2021-05-01 at 5 12 56 PM (1)](https://user-images.githubusercontent.com/82637289/116854175-cfad4900-abe6-11eb-8870-302176035f47.jpeg)

![WhatsApp Image 2021-05-01 at 5 12 57 PM](https://user-images.githubusercontent.com/82637289/116854129-b86e5b80-abe6-11eb-8b47-2f98cc2c920b.jpeg)
