# **apache-kali-linux-Setup-portforwarding**

# Setup Apache

sudo apt update
sudo apt install apache2

You have now apache in your Kali. Now start apache by using 

sudo systemctl start apache2

Enable apache on boot (Optional)

sudo systemctl enable apache2

(If you want to disable apache on boot use sudo systemctl disable apache2)

now you have started apache, go to http://localhost so make sure your apache is started locally. 

![Screenshot From 2025-06-01 09-28-20](https://github.com/user-attachments/assets/d3a31810-d838-4ad2-a325-dbbf6845c2ec)

your html files in localhost is in /var/www/html/  you can replace to your html file if you want. 


**Port Forwarding**

Now your html is hosting locally, time to do port fowarding so everywhere in the internet can see it. 

Go check your home router and router's setting adress( http:// yoursettingipadress) and Sign-in information(username and password). If you couldn't found your sign-in infomation, contact your ISP. 

in your home router go to access controll and port forwarding, and configure...

Protocol: TCB

External Port and Internal Port: 80 (since we'll be using http as protocol)

internal host: Your ip adress

to check your ip adress, use ip a to find your subnet ip adress. 

For Wi-Fi user, check your wlan and find inet. For LAN user, check your eth and find inet. <-example->  inet 192.168.1.0/24

Delete /24 and paste that to internal host.
Save the setting and type http:// YourPublicIPAdress, no need to type :80
