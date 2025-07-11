# Sea-Vessels-Detector

Проект по прикладному машинному обучению трех студентов НГУ (2 курс, 4 семестр).
## Описание

Автоматический поиск судов, совершающих незаконные маневры и швартующихся в неположенных местах (судно в определенной зоне).
### Основные функции

1. Обнаружение плавсредств в акватории портовых городов
2. Классификация найденных судов
3. Обнаружение и классификация правонарушений на видео, если они присутствуют в кадре.
## Обученные модели

### YOLOv8

Универсальный фреймворк для обнаружения и классификации объектов на изображении. Обладает высокой скоростью и точностью, что полезно для потокового видео с камер наблюдения.
### Основные классы

1. Внутренние
2. Транспортные
3. Специальные
4. Яхта
5. Гидроциклы
6. Лодка
## Результаты обучения
### 1. Общая информация

- **Модель**: YOLOv8m
- **Датасет**: Собственный, количество изображений в train - 6076 и val - 1518
- **Количество эпох**: 450
- **Выход на плато**: 179
- **Размер изображений**: 640x640
- **Аугментации**: В обучении использовалась аугментация с настройками: цветовые искажения (HSV), повороты, сдвиги, масштабирование, mosaic, mixup и copy-paste.
### 2.1 Метрики по задачам

- **mAP0.5**: 0.909
- **mAP0.5-0.95**: 0.769
- Precision: 0.909
- Recall: 0.845
- Точность по каждому классу:
	1. Indastrial - 0.921
	2. Transport - 0.935
	3. Special - 0.945
	4. Yaht - 0.905
	5. Hydrosycles - 0.967
	6. Boat - 0.779
### 2.2 Визуализация
- Графики
	![Graffics](https://github.com/BodgeDook/Sea-Vessels-Detector/blob/main/assets/results.png)
- Пример работы
	![Retult on validation part](https://github.com/BodgeDook/Sea-Vessels-Detector/blob/main/assets/val_batch1_pred.jpeg)
	![Result on video](https://github.com/BodgeDook/Sea-Vessels-Detector/blob/main/assets/results.gif)
	
