# Postman - Quick Installation for Debian/Ubuntu

👉 Simply **copy the entire block below** and paste it into your terminal:

```bash
sudo rm -rf /opt/Postman

curl -L https://dl.pstmn.io/download/latest/linux64 -o /tmp/postman.tar.gz && \
tar -xzf /tmp/postman.tar.gz -C /tmp && \
sudo mv /tmp/Postman /opt/ && \
rm /tmp/postman.tar.gz

sudo tee /usr/share/applications/postman.desktop > /dev/null <<EOF
[Desktop Entry]
Encoding=UTF-8
Name=Postman
Exec=/opt/Postman/Postman
Icon=/opt/Postman/app/resources/app/assets/icon.png
Terminal=false
Type=Application
Categories=Development;
EOF
```

## What this script does:

1. Removes any existing Postman installation from `/opt/Postman`
2. Downloads the latest Postman version for Linux
3. Extracts and installs it to `/opt/Postman`
4. Creates a desktop entry for easy application launcher access
5. Cleans up temporary files

After installation, you can launch Postman from your application menu.
