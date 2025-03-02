# Практическая работа 1. Git

## Как создать новый репозиторий на [GitHub](https://github.com 'Гитхаб!!!') и работать с ним.
---
### 1. Создаешь новый репозиторий на GitHub (например first-repo)
### 2. У себя на компьютере:
##### Если у тебя есть проект, переходишь в корень проекта, если хочешь новый проект, то:
``` mkdir first-repo  
cd first-repo  
git init
```
* Создали каталог first-repo
* Перешли в него
* Инициализировали репозиторий (сделали из папки репозиторий)

### 3. Добавляешь связь с [GitHub](https://github.com) 
```
git remote add origin git@github.com:Nmplz/first-repo.git
```
##### origin - имя ссылки на удалённый перезиторий ( может быть любым, но обычно используют стандартное название)

### 4. Создаешь файлы, коммитишь
```
echo "# First-repo" > README.md
git add README.md
git commit -m "first commit"
```
##### ключ -m задает описание коммита, и, на сколько я понял, является обязательным.

### 5. Отправляешь

``` git push -u origin  master ```
##### 
* git push - отправка изменений в удалённый репозиторий
* -u связь локальной ветки с удалённой
* origin - Имя удалённого репозитория
* master/main - Название ветки.

# Конец.