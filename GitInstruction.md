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