# minecraft_server

# ブラウザでhttps://www.minecraft.net/ja-jp/download/serverからサーバープログラムをダウンロード
LANG=C xdg-user-dirs-gtk-update
sudo apt update
sudo apt upgrade
sudo apt install openjdk-19-jdk-headless
sudo apt install openssh-server
sudo systemctl enable ssh --now
udo ufw enable
sudo ufw allow 22
sudo ufw allow 25565
sudo ufw allow 25575

# java -Xms1024M -jar server.jar nogui
