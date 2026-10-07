# Tạo

sudo vim /etc/nginx/sites-available html.giangngocthanh.com.conf

# Link

sudo ln -s /etc/nginx/sites-available/tenfile.conf /etc/nginx/sites-enabled
sudo ln -s /etc/nginx/sites-available/jenkins.giangngocthanh.bid.conf /etc/nginx/sites-enabled




# Unlink

sudo rm -rf tenfile
sudo rm -rf /etc/nginx/sites-enabled

# check cú pháp & reload

sudo nginx -t
sudo systemctl reload nginx

sudo vim giangngocthanh-private.key
sudo vim giangngocthanh-public.crt
