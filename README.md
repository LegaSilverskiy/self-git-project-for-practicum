
#Git и консольные команды
/System/Volumes/Data/Users/olegserebranskij/
1) *pwd* - узнать в какой директории ты находишься
2) *cd ~* - перейти в домашнюю директорию
3) *ls* - узнать содержимое директории
3.1) *ls -a* - узнать содержимое директории + отобразит скрытые файлы
3.2) *ls ~* - выведет содержимое домашней директории вне зависимости от того что покажет pwd
3.3) *ls ..* - выведет содержимое родительской папки
«Если в названии папки есть пробелы, при вводе нужно использовать кавычки»
4) *cd ..* - вернуться в родительскую директорию
5) *touch %ИМЯ_ФАЙЛА%* - создать файл(можно создать сразу несколько файлов, если указать их через)
6) *mkdir* - создать директорию
7) *mkdir -p (mkdir -p dir1/dir-inside/dir-deeper-inside)* - создать структуру директорий

Также можно использовать обе команды вместе с символом домашней директории (~) или родительской директории (..). Например, команда mkdir ~/my-git-projects создаст папку my-git-projects внутри домашней директории.
А команда touch ../../file.txt создаст файл file.txt на две папки выше по иерархии. Допустим, если вы находитесь в директории projects/git/hello, команда touch ../../file.txt создаст файл по такому пути: projects/file.txt.

8) *cp что_копируем куда_копируем* - скопировать (можно копировать сразу несколько файлов, если указать по порядку «что_копируем» и в конце указать директорию)
9) *mv* - перенести папку в другое месту (синтаксис аналогичен команде cp)
10)*cat* - прочитать файл в терминале
11)*rm* - удалить файл
11.1)*rmdir* - удалить директорию
11.2)*rm -r* - удалить директорию вместе с содержимым, если директория не пустая
! Команды в терминале необязательно вбивать и выполнять по очереди. Их можно указывать не по одной, а сразу списком. Для этого их нужно разделить двумя амперсандами (&&).
$ mkdir second-project && cd second-project && touch index.html style.css
 создаём папку second-project,
 переходим в папку second-project
 и создаём в ней два файла: index.html и style.css 
 
 ---
#GIT
1)*git init* - инициализировать репозиторий в папке, в которой вы сейчас находитесь
1.1)*rm -rf .git* - удалить ранее созданый гит репозиторий
2)*git status* - проверить состояние репозитория
Команда git status выведет:
    название текущей ветки: On branch master или On branch main;
    сообщение о том, что в репозитории ещё нет коммитов: No commits yet;
    сообщение, которое говорит: «чтобы что-нибудь закоммитить (то есть зафиксировать), нужно сначала это создать» — nothing to commit (create/copy files and use "git add" to track).
3)*git add* - добавить файл(подготовить к Сохранению в гит)
    Команда git add позволяет подготовить файл к сохранению.
    Команда git add --all подготовит к сохранению сразу все файлы.
    С помощью git add . можно добавить в репозиторий текущую папку со всеми файлами.
4) *git commit* - сделать коммит(сохранить изменения в гит)
    Коммит можно сделать с помощью команды git commit.
    Ключ -m позволяет присвоить коммиту сообщение. Помните, что такие сообщения должны быть информативными: чётко описывать изменения.
    В коммит попадает то, чтобы было предварительно добавлено «в корзину», или «в кадр», перед коммитом.
5)*git log* - посмотреть историю коммитов
6)*git push* - запушить изменения в гитхаб


##Добавляю ссылку на [гугл](https://www.google.com)


##Добавляю код


```swift
var a = "Hello, world!"
print(a)
```
