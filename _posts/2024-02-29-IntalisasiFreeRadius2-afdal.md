# freeradius
## update
sudo apt update
## install aplikasi
sudo apt install freeradius freeradius-mysql freeradius-utils
From <https://kifarunix.com/install-freeradius-with-daloradius-on-ubuntu-20-04/?expand_article=1>
## cek insalasi
sudo systemctl stop freeradius

sudo freeradius -X
### pastikan
Ready to process requests
### hentikan proses : Ctrl+ C
### jalankan service lagi
systemctl enable --now freeradius
## Atur firewal jika perlu
ufw allow to any port 1812 proto udp
ufw allow to any port 1813 proto udp
## cek servise
sudo systemctl start freeradius
sudo systemctl enable freeradius
sudo systemctl status freeradius
## menambah user
sudo nano /etc/freeradius/3.0/users
john Cleartext-Password := "coba1234"
simpan
sudo systemctl restart freeradius
## mengetes
 Quick Notes Page 1
radtest john coba1234 localhost 0 testing123
## menambah client nas mikrotik di free radius
sudo nano /etc/freeradius/3.0/clients.conf
client mikrotik {
 ipaddr = 192.168.200.1
 secret = testing123
 shortname = mikrotik_client
 nastype = mikrotik
}
restart
sudo systemctl restart freeradius
## tambahan
chmod 2755
From <https://help.univention.com/t/freeradius-will-not-start/13476>
## dalo radius
https://kifarunix.com/install-freeradius-with-daloradius-on-ubuntu-20-04/?expand_article=1

## Gambar hasil kegiatan:

![Capture](https://github.com/akusukacoding22/riannnnnn/assets/156275570/4f02dd5b-b5b6-4def-91ba-bd594809db42)

