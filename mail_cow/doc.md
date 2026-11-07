```bash
sudo hostnamectl set-hostname mail.giangngocthanh.bid

dig @1.1.1.1 +short mail.giangngocthanh.bid
dig @1.1.1.1 MX giangngocthanh.bid +short

sudo -i

umask 0022
cd /opt
git clone https://github.com/mailcow/mailcow-dockerized
cd mailcow-dockerized

./generate_config.sh

# Mail server hostname ... hostname: mail.vulebaolong.com
# Timezone [Etc/UTC]: Asia/Ho_Chi_Minh
# Branches: 1

# cd /opt/mailcow-dockerized
docker compose pull
docker compose up -d

```
