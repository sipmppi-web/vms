bash <(curl -s https://raw.githubusercontent.com/SuccessJII/VPS-Youtube/refs/heads/main/main.sh)

cd .idx
bash vm.sh

depois, faça isso

sudo su
apt update
apt install dropbear -y
dropbear -p 22
Playit: https://playit.gg/
curl -SsL https://playit-cloud.github.io/ppa/key.gpg | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/playit.gpg >/dev/null
echo "deb [signed-by=/etc/apt/trusted.gpg.d/playit.gpg] https://playit-cloud.github.io/ppa/data ./" | sudo tee /etc/apt/sources.list.d/playit-cloud.list
sudo apt update
sudo apt install playit

playit start 
