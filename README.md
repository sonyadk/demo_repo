___
### git config 

Может быть использована для указания пользовательских настроек, таких как электронная почта, имя пользователя, формат и т.д

git config --global user.email адрес@gmail.com
___

### git difftool 
Запускает внешнюю утилиту сравнения для показа различий в двух деревьях.

git difftool --tool-help
___

### git discard 
Позволяет не отправлять в репозиторий те изменения которые нам не нравятся.

git checkout -p
___

### git revert 
Позволяет откатить существующие комиты.

git revert <commit>
___

### git hard reset 
Позволяет откатить целую пачку комитов.

git reset -hard 
___

### git remote 
Команда позволяет пользователю подключиться к удаленному репозиторию.

git remote -v origin
___

### git tag 
Используется для маркировки определенных коммитов с помощью простых меток.

git tag 1.1.0 <вставьте-commitID-здесь>
___

### git log 
Отобразит список всех коммитов в ветке вместе с соответствующими сведениями.

git log --oneline – показывает каждый коммит в одной строке. Кроме того, она показывает лишь префикс ID коммита.
git log --decorate печатает все относительные имена показанных коммитов
___

### git stash 
Помогает в сохранении изменений на временной основе, эти изменения не попадут в коммит сразу.

git stash
___

### git show 
Для просмотра информации о любом git объекте.

git show
___

### git fetch 
Позволяет пользователю доставить все объекты из удаленного репозитория, которые не присутствуют в локальном рабочем каталоге.

git fetch origin
___

### git ls-tree 
Используется для просмотра дерева объекта вместе с названием, режимом каждого предмета и значением SHA-1.

git ls-tree -r HEAD
___

### git cat-file 
Просмотреть тип объекта с помощью SHA-1 значения. 

git cat-file –p d670460b4b4aece5915caf5c68d12f560a9fe3e4

git cat-file -p HEAD
___

### git grep 
Позволяет пользователю проводить поиск фраз и слов в содержимом деревьев.

git grep "www.hostinger.ru"
___

### git gc
Поможет удалить и оптимизировать ненужные файлы

git gc
___

### git archive 
Позволяет пользователю создать .zip или .tar файл содержащий компоненты одного из деревьев репозитория. 

git archive --format=tar master

git archive -o update.zip HEAD $(git diff --name-only --diff-filter=d HEAD^..HEAD)
___



