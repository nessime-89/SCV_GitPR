[Alt text](kisspng-computer-icons-pro-git-portable-network-graphics-i-git-book-pro-git-app-app-5b80546c0b1311.5417567715351368760454.jpg)
# Работа с Git и GitHub
## 1. Проверка наличия установленного Git
Выполнить в терминале команду ``git version``.
Если Git установлен, появится сообщение с информацией о версии программы. Иначе выйдет сообщение об ошибке
## 2. Установка Git
Загружаем последнюю версию Git с официального сайта [сайт](https://git-scm.com/downloads).
Устанавливаем с настройками по умолчанию.
## 3. Настройка Git
При первом использовании необходимо представиться
```
git config --global user.name «Ваше имя английскими буквами»

git config --global user.email ваша почта@example.com
```
## 4. Инициализация репозитория
Чтобы инициализировать репозиторий в терминале выполняем комманду ``git init``. Выполняем 1 раз при создании папки
## 5. Запись изменений в репозитории
Для того, чтобы записать изменения выполнить комманду в терминале ``git add .`` - если одна папка. Или ``git add название файла`` и кнопка таб - для корректной подстановки запроса.
Далее вводим в терминале ``git commit -m "текст комментария"`` - чтобы ввести комментарий к изменению.
## 6. Просмотр истории коммитов
Для вывода на экран истории всех коммитов с их хеш-кодами необходимо ввести команду в терминале ``git log``.
``git log --oneline`` - для того чтобы вывести историю в более короткой версии.
``git log --graph`` - для просмотра веток.

## 7. Перемещение между сохранениями 
Комманды для перехода между версиями сохранений
``````
git checkout идентификатор из логов – переход от одного коммита к другому
git checkout master – вернуться к актуальному состоянию и продолжить работу
git switch -(тире)  - для того чтобы вернуться к последней актуальной версии
``````
## 8. Игнорирование файлов
Для того, чтобы исключить из отслеживания в репозитории определенные файлы или папки, необходимо создать там файл ***.gitignore*** и записать в него их названия или шаблоны, соответствующие таким файлам или папкам. (чтобы скрыть картинку, убрать перед ссылкой на картинку ! и наоборот добавить его, чтобы картинка появилась)
## 9. Создание веток в Git
Создать ветку можно командой:
```
git branch <имя новой ветки>
git checkout -b <имя новой ветки>
git switch -c <имя новой ветки>
```
По умолчанию имя основной ветки в Git - *master*.
Список веток в репозитории можно посмотреть с помощью команды 
```
git branch
```
## 10. Слияние веток и разрешение конфликтов
Для слияния выбранной ветки с текущей нужно выполнить команду:
```
git merge <название выбранной ветки>
```
Если была изменена одна и та же часть файла в обеих ветках, может возникнуть конфликт, который потребует участия пользователя. VSCode предлагает варианты разрешения. Чтобы разрешить конфликт, необходимо выбрать один из вариантов, либо объединить содержимое по-своему.
После сохранить изменения с помощью **git commit -am "комментарий к изменению"**
## 11. Удаление ветки
Необходимо перейти в любую другую ветку, чтобы не вышла ошибка при выполнении команды **git checkout <название ветки> или git switch <название ветки>**
Для удаления выполнить:
```
git branch -d <название ветки которую удаляем>
git branch -delete <название ветки которую удаляем>
```
Если вместо d написать D - выполнится принудительное действие (все заглавные буквы в Git)

# ***Работа с удаленными репозиториями***
1. Создать аккаунт на GitHub
2. Создать локальный репозиторий
3. Создать удаленный репозиторий на GitHub
4. Связать удаленный репозиторий с локальным

Добавить удаленный репозиторий к проекту:
```
git remote add <имя для репозитория (обычно принято писать origin)> <url-адрес репозитория в сети>
```
Для получения и слияния изменений из удаленного репозитория используем команду:
```
git pull
```
Для того, чтобы внести изменения в аккаунт на GitHub используем команду
```
git push
```
Инструкция по созданию копии копии чужого репозитория и предложения своей версии во вкладке (папке) SCV_GitPR - README.md

# Репозиторий для **pull request**
* В своём аккаунте на GitHub создать копию репозитория **"AndreyBulgakov19/SCV_GitPR"** с помощью кнопки **"Fork"**.
---
* Клонировать копию репозитория на локальный компьютер.
---
* Создать новую ветку.
---
* Добавить файл с инструкцией в новую ветку.
---
* Дополнить инструкцию разделами по работе с удалёнными репозиториями, pull request.
---
* Зафиксировать изменения (коммиты).
---
* Отправить изменения на GitHub.
---
* На сайте GitHub выполнить **Pull request**.
---