# BEERecommend
![](https://gitlab.com/goto-ru/appliedprog/school-2017.10-spb/BEERecommend/raw/master/images/BEERecommend.png)
*******
# Идея 
Идея заключалась в создании рекомендательной системы алкогольных напитков. В данном случае рекомендательной системы пива. 
*******
# Мотивация
Сделать рекомендательную систему, решить проблему холодного старта. Разобраться с поэтомным решение этих задач.
*******
# Сделано
Реализванные две рекомендательные системы. Так же реализован веб-сервис, который использует первую рек. систему и собирает информацию для второй. Данные для создания "фичей" пива были взяты с сайта BJCP.org . Так как никакой информации о пользовательских предпочтениях у нас нет, мы ранжируем сорта пива по расстояниям в некотором пространстве (компоненнты сжаты с помощью TruncatedSVD), вообщем KNN, тем самым обеспечивая пусть и не самые лучшие рекомендации, но работоспособность сервиса и сбор информации для модели с Коллаборативной фильтрацией. После сбора необходимого кол-ва данных в сайт будет интегрированна вторая модель, выполняющая задачу рекомендации лучше.
*******
# Результат
Написаны две рекомендательные системы. Реализован некоторый веб-сервис.
*******
# Планы
Доделать веб-сервис, так как имеюся некоторые проблемы с оформлением и разными разрешениями устройств. Интегрировать вторую модель в веб-сервис.
*******
# Как использовать Web_part
Требуется установить ряд библиотек:
	
1. django
	
2. django-widjet-tweaks
	
3. numpy
	
4. pickle

для скачивания проекта и запуска localhost'а:
******
```
#Cloning repo

$ git clone https://github.com/Punctuality/BEERecommend

#No comments

$ cd BEERecommend/Web_part/

#Activating venv

$ source ../venv/bin/activate

#Running server

$ python3 manage.py runserver
```

That's all!
******
[GitLab Repository](https://gitlab.com/goto-ru/appliedprog/school-2017.10-spb/BEERecommend/tree/master)
