# Начало работы с GitHub

## 1. Создание ssh-ключа
Cоздаём ключ
```
ssh-keygen -t ed25519 -C "email@here.com"
```
Добавляем ключ в ssh-agent:
```
ssh-add ~/.ssh/id_ed25519
```

## 2. Добавление ключа на гитхаб
Настройки профиля -> вкладка SSH and GPG keys ->  нажать Add ssh key.
Копируем туда содержимое файла ~/.ssh/id_ed25519.pub и нажимаем Add

## 3.Клонирование репозитория
Вводим команду:
```
git clone <ssh-url> -d <directory>
```
