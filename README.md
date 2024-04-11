# pryzm-g-ncelleme
systemctl stop pryzmd
wget https://storage.googleapis.com/pryzm-zone/core/0.13.0/pryzmd-0.13.0-linux-amd64
chmod +x pryzmd-0.13.0-linux-amd64
mv pryzmd-0.13.0-linux-amd64 $(which pryzmd)
systemctl restart pryzmd
journalctl -u pryzmd -fo cat
