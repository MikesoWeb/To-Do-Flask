Простой ToDo менеджер, реализованный на веб-фреймворке Flask
В качестве веб-интерфейса использован фреймворк Semantic UI https://semantic-ui.com/

![Image alt](https://sun9-87.userapi.com/s/v1/ig2/qoOIVsuNQnj2xPLBAtjqlJAA2V8widKcpeGjC8bwy3qCKQ_JAQsQFUwLkc31mSQaYNIun91Pw8QDfPeworrJ_xk1.jpg?size=1280x827&quality=96&type=album)

**UPD 1.0**  от  _5.13.22_

    Добавлен файл config.py и туда перенесена конфигурация приложения
    Добавлен модуль python-dotenv и файл .env для хранения значений переменных окружения приложения
    


**Внимание!** 
Файл .env должен быть указан в файле .gitignore чтобы ваши настройки не улетели в репозиторий
Для данного примера я его исключил из файла игнора




Создаем папку для нового проекта и переходим в нее

    md ToDoFlask & cd ToDoFlask

Устанавливаем и активируем виртуальное окружение

    python3 -m venv venv
    . venv/bin/activate


Активируем git
    
    git init


Создаем файлы и папки в проекте
    
    md todo & cd todo
    md templates
    mkdir static\css
    echo .> templates/layout.html
    echo .> templates/index.html
    echo .> static/css/style.css

    cd ..
    copy con .gitignore
    copy con README.MD
    copy con app.py


Устанавливаем flask и ORM SQLAlchemy

    pip install Flask Flask-SQLAlchemy


Создаем файл с зависимостями проекта

    pip freeze > requirements.txt


Устанавливаем переменные окружения 
    
для bash

    export FLASK_APP=app.py
    export FLASK_ENV=development

для cmd

    set FLASK_APP=app.py
    set FLASK_ENV=development


Запускаем приложение
    
    flask run




- [Ссылка на оригинал](https://youtu.be/3vfum74ggHE)
- [Ссылка на видео с моего канала по данному примеру](https://youtu.be/dsI_a63pFws) 
    
    Терехов Михаил 2022 год
