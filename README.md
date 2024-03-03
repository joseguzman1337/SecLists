# For Debian, Ubuntu, Kali or Parrot
```
if [ ! -d "/usr/share/wordlists" ]; then sudo mkdir /usr/share/wordlists; fi && \
apt update -y && \
apt install git -y && \
[ -d "/usr/share/wordlists" ] && { sudo mv /usr/share/wordlists /usr/share/wordlists_bck || true; } && \
git clone https://github.com/4k4xs4pH1r3/SecLists.git /usr/share/wordlists && \
[ -d "/usr/share/wordlists_bck" ] && { cd /usr/share/wordlists_bck/ && sudo mv * -u -f /usr/share/wordlists/ || true; } && \
cd /usr/share/ && \
git clone https://github.com/danielmiessler/SecLists.git /usr/share/SecLists && \
cd && \
apt install neofetch screenfetch -y && \
neofetch && \
apt install nmap metasploit-framework asciinema steghide radare2 mtr firmware-realtek net-tools wpasupplicant wireless-tools -y && \
screenfetch && \
apt-get autoclean && \
apt install -f && \
apt -f install && \
apt autoremove -y && \
apt-get clean cache && \
apt update && \
apt-get autoclean && \
apt-get clean cache && \
apt update && \
apt update -y && \
apt full-upgrade -y --allow-downgrades && \
sudo dpkg --configure -a && \
cd && \
sudo apt-get install python python3 python-pip python3-pip python-dev python-setuptools -y && \
neofetch && \
bash <(wget -qO- https://git.io/vAtmB)
```

# For macOS
```
cd && mkdir ~/wordlists && sudo git clone https://github.com/4k4xs4pH1r3/SecLists.git ~/wordlists && mkdir ~/SecLists && sudo git clone https://github.com/danielmiessler/SecLists.git ~/SecLists && brew install neofetch && neofetch
```
