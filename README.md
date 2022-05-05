This is an educational repository that contains homeworks, completed as part of Vadim Ksendzov's training course on software testing. 
Here I am learning how to work in GitHub. 
Below is my homework and solution
# TXT

### Создать внешний репозиторий c названием TXT:

`https://github.com/demiurgusnen9/TXT.git`

### Клонировать репозиторий TXT на локальный компьютер:
```
  $ git clone https://github.com/demiurgusnen9/TXT.git
  Cloning into 'TXT'...
  remote: Enumerating objects: 3, done.
  remote: Counting objects: 100% (3/3), done.
  remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
  Receiving objects: 100% (3/3), done.
```
### Внутри локального TXT создать файл “new.txt”:

```
  $ cd TXT
  $ touch new.txt
```

### Добавить файл под гит:
`
  $ git add new.txt
`
### Закоммитить файл:
```
  $ git commit -m "add new.txt"
  [main d42955c] add new.txt
  1 file changed, 0 insertions(+), 0 deletions(-)
  create mode 100644 new.txt
```
### Отправить файл на внешний GitHub репозиторий:
```
   $ git push
    Enumerating objects: 4, done.
    Counting objects: 100% (4/4), done.
    Delta compression using up to 2 threads
    Compressing objects: 100% (2/2), done.
    Writing objects: 100% (3/3), 274 bytes | 274.00 KiB/s, done.
    Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
    To https://github.com/demiurgusnen9/TXT.git
    60aa8a0..d42955c  main -> main
```

### Отредактировать содержание файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT.
```
   $ vim new.txt
   ФИО - Masalskaya Alena Viktorovna
   Возраст - 30
   Количество домашних животных - 1
   Будущая желаемая зарплата - 500$
```

### Отправить изменения на внешний репозиторий.
```
   $ git commit -am "add info in new.txt"
    warning: LF will be replaced by CRLF in new.txt.
    The file will have its original line endings in your working directory
    [main c7bb0d8] add info in new.txt
     1 file changed, 4 insertions(+)

   $ git push
    Enumerating objects: 5, done.
    Counting objects: 100% (5/5), done.
    Delta compression using up to 2 threads
    Compressing objects: 100% (3/3), done.
    Writing objects: 100% (3/3), 429 bytes | 429.00 KiB/s, done.
    Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
    To https://github.com/demiurgusnen9/TXT.git
    d42955c..c7bb0d8  main -> main
```

### Создать файл preferences.tx:
`
   $ touch preferences.txt
`

### В файл preferences.txt” добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате TXT:
```
   $ vim preferences.txt
   Любимый фильм - Трудности перевода
   Любимый сериал - Клиника
   Любимая еда - Кукурузные_палочки
   Любимое время года - Зима
   Страна которую хотели бы посетить - Исландия
```

### Создать файл sklls.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT
```
   $ vim skills.txt

   1. Базовая теория (Что такое тестирование, багрепорты, документация, виды, методы, направления тестирования и т.п.) SDLC, STLC.
   2. Что такое клиент-серверная архитектура.
   3. HTTP Методы запросов на сервер.
   4. Коды ответов HTTP сервера.
   5. Структуры HTTP запросов и ответов.
   6. Что такое JSON, XML. Их структура.
   7. Тестирование API через Postman (JS, автотесты API).
   8. Снятие и чтение логов c внешнего сервера.
   9. Снифинг http web трафика через Charles и Fiddler.
   10. Dev Tools веб браузеров (Google Chrome, FireFox).
   11. VPN. (Как работает, зачем нужен, как использовать, варианты инструментов)
   12. Мобильное тестирование.
   13. Особенность iOS, Android, гайдлайны.
   14. Сборка iOS приложений на XCode. (У кого нет Mac компьютера, просто посмотрят)
   15. Сборка Android приложений на Android Studio.
   16. ADB (управление андройд девайсами).
   17. Настройка прокси и vpn на iOS и Android.
   18. Перехват (сниффинг) мобильного трафика через Charles и Fiddler на iOS и Android.
   19. Командная строка (terminal) Linux (копирование, создание, просмотр, перемещение файлов на серверах без графического интерфейса)
   20. Основы bash скриптинг, автоматизация рутинных задач на сервере.
   21. Доступ к удалённым серверам.
   22. Основы SQL (Create, Delete, Drop, Insert Into, Select, From, Where, Join).
   23. База данных Postgres (установка, настройка и использование).
   24. Нереляционная база данных Redis (установка, настройка и использование).
   25. Нагрузочное тестирование в Jmeter.
   26. Методология разработки Scrum.
   27. Python. (Изучение основ. Создание клиент серверного приложения)
```

### Сделать коммит в одну строку:
```
   $ git add . && git commit -m "add preferences.txt and skills.txt with info"

    warning: LF will be replaced by CRLF in preferences.txt.
    The file will have its original line endings in your working directory
    warning: LF will be replaced by CRLF in skills.txt.
    The file will have its original line endings in your working directory
    [main 07e1510] add preferences.txt and skills.txt with info
     2 files changed, 32 insertions(+)
      create mode 100644 preferences.txt
       create mode 100644 skills.txt
```

### Отправить сразу 2 файла на внешний репозиторий.
```
   $ git push
    Enumerating objects: 5, done.
    Counting objects: 100% (5/5), done.
    Delta compression using up to 2 threads
    Compressing objects: 100% (4/4), done.
    Writing objects: 100% (4/4), 1.62 KiB | 830.00 KiB/s, done.
    Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
    To https://github.com/demiurgusnen9/TXT.git
      c7bb0d8..07e1510  main -> main
```

### На веб интерфейсе создать файл bug_report.txt:
`
   done
`
### Сделать Commit changes (сохранить) изменения на веб интерфейсе:
`
   done
`

### На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT:
```
   ID:ID
   Summary:Короткое описание
   Steps to Reproduce: Шаги воспроизведения
   Expected Result:Ожидаемый результат
   Actual Result:Фактический результат
   Severity:Серьезность	
```

### Сделать Commit changes (сохранить) изменения на веб интерфейсе.
`
   done
`

### Синхронизировать внешний и локальный репозиторий TXT
```
   $ git pull
    remote: Enumerating objects: 7, done.
    remote: Counting objects: 100% (7/7), done.
    remote: Compressing objects: 100% (5/5), done.
    remote: Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
    Unpacking objects: 100% (6/6), 1.43 KiB | 81.00 KiB/s, done.
    From https://github.com/demiurgusnen9/TXT
    07e1510..c8bdb39  main       -> origin/main
    Updating 07e1510..c8bdb39
    Fast-forward
    bug_report.txt | 6 ++++++
    1 file changed, 6 insertions(+)
    create mode 100644 bug_report.txt
```
