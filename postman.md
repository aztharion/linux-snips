# Debian/Ubuntu - Cài nhanh Postman

👉 Người dùng chỉ việc **copy toàn bộ block bên dưới** và paste vào terminal:

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
