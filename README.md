<h1>How To Install Nginx on Ubuntu 20.04</h1>

<h4>sudo apt update</h4>

<h4>sudo apt install nginx</h4>

<h4>sudo ufw app list</h4>


<h4>sudo ufw allow 'Nginx HTTP'</h4>


<h4>sudo ufw status</h4>

<h4>systemctl status nginx</h4>

<h4>sudo systemctl stop nginx</h4>

<h4>sudo systemctl start nginx</h4>

<h4>sudo systemctl restart nginx</h4>

<h4>sudo systemctl enable nginx</h4>

<h4>sudo systemctl disable nginx</h4>

sudo mkdir -p /var/www/your_domain/html

sudo chown -R $USER:$USER /var/www/your_domain/html

sudo chmod -R 755 /var/www/your_domain

sudo nano /var/www/your_domain/html/index.html

sudo nano /etc/nginx/sites-available/your_domain

sudo ln -s /etc/nginx/sites-available/your_domain /etc/nginx/sites-enabled/

sudo nano /etc/nginx/nginx.conf

sudo nginx -t

sudo systemctl restart nginx
