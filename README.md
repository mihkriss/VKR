## Описание 
Сервис для выявление драк в реальном времени с помощью искусственного интелекта

## Общая схема и принцип работы
1. Составление датасета:
   1. Готовый датасет из видео с драками: https://www.kaggle.com/datasets/mohamedmustafa/real-life-violence-situations-dataset
   2. Нарезание видео на кадры по 10 частей для сбалансированности классов
   3. YOLOv8n-pose извлечение ключевых точек из объектов на кадров
   4. Составление датафрейма data.cvs для обучения модели (доп. параметры: метки на позу из кадра, параметр расстояние между объектами)
      
2. Разработка нейронной сети:
     1. Предварительная обработка данных для обучение модели
     2. Составление архитетуры нейронной сети
     3. Оценка метрик
     
3. Разработка сервиса для внедрение обученной модели:
   1. Общий вид сервиса
   2. Виджет с видеопотоком
   3. Виджет с картой для определения положения съемки
   4. База данных для хранения информации об объектах из кадра 






https://github.com/mihkriss/VKR/assets/74809078/17b6c79e-9a13-43cf-b8ae-7350806a3040

