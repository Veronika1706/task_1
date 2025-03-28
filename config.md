[< назад](readme.md)

# Базовая настройка GIT

Прежде всего, чтобы приступить к работе с Git, необходимо установить его на компьютер, затем произвести базовые настройки.

[Инструкция для скачивания и установки](https://git-scm.com/)

После установки GIT следует выполнить базовую настройку окружения. Эта процедура выполняется один раз на каждом устройстве, но при необходимости можно внести изменения, используя те же команды.

### Установка имени и электронной почты

Выполните следующие команды, чтобы Git узнал ваше имя и электронную почту. Эти данные используются для подписи изменений сделанных вами, что позволит отслеживать, кто и когда сделал изменения в файле.

```
git config --global user.name "Your Name"
git config --global user.email "your_email@whatever.com"
```

### Имя ветки по умолчанию

Чтобы установить имя ветки, которое будет использоваться по умолчанию, выполните следующую команду:

```
git config --global init.defaultBranch main
```

### Корректная обработка окончаний строк

Для пользователей Unix/Mac:

```
git config --global core.autocrlf input
git config --global core.safecrlf warn
```

Для пользователей Windows:

```
git config --global core.autocrlf true
git config --global core.safecrlf warn
```

***В конце настройки можно проверить как сохранились внесенные изменения выполнив следующую команду:*** 

```
git config --list
```