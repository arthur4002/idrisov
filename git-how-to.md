#создаем public/private key
ssh-keygen -t ed25519 -C "your_email@example.com" 

#добавляем приватный ключ в ssh-agent
ssh-add ~/.ssh/id_ed25519 

--------------------------------
#Добавляем публичный ключ в github в настройках


-----------------------------------
#Инициализируем пользователя git
git config --global user.name "username"
git config --global user.email "email"

#Подключаемся по приватному ключу к github
ssh -T git@github.com
git init
git remote add origin git@github.com:arthur4002/idrisov.git


