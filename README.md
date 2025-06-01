# Apache-kali-linux-Setup-portforwarding
Apache is a widely-used web server software that allows you to host websites and web applications. 

#Install Apache

sudo apt update
sudo apt install apache2

#You have now apache in your Kali. Now start apache by using 

sudo systemctl start apache2

#Enable apache on boot (Optional)

sudo systemctl enable apache2

(If you want to disable apache on boot use sudo systemctl disable apache2)

#now you have started apache, go to http://localhost so make sure your apache is started locally.  ![Screenshot From 2025-06-01 09-28-20](https://github.com/user-attachments/assets/d3a31810-d838-4ad2-a325-dbbf6845c2ec)

#your html files in localhost is in /var/www/html/  you can replace to your html file if you want. 


**Port Forwarding**
#
