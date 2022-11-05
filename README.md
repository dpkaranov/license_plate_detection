# license_plate_detection

## Описание экспериментов

### Эксперимент №1 "Обучение Inception-ResNet-v2"

Inception-ResNet-v2 — это сверточная нейронная сеть, обученная на более чем миллионе изображений из базы данных ImageNet. Сеть состоит из 164 слоев и может классифицировать изображения по 1000 категориям объектов, таким как клавиатура, мышь, карандаш и т.д. Inception-ResNet-v2 используется в основном для задачи классификации. Архитектура сети показана ниже.

<image src="./images/imagenet.png"></image>

### Метрики Inception-ResNet-v2

<image src="./images/resnetv2_metrics.png"></image>

### Эксперимент №2 "Обучение YOLOv5"

YOLO или «Только один раз взгляните» — это один из наиболее широко используемых алгоритмов обнаружения объектов, основанных на глубоком обучении. YOLO делит изображение на сетку, и каждая сетка обнаруживает объекты внутри себя. Их можно использовать для обнаружения объектов в реальном времени на основе потоков данных. Они требуют очень мало вычислительных ресурсов. Она состоит из трех частей: (1) Хребет: CSPDarknet, (2) Шея: PANet и (3) Голова: Yolo Layer. Данные сначала вводятся в CSPDarknet для извлечения признаков, а затем передаются в PANet для слияния признаков. Наконец, Yolo Layer выводит результаты обнаружения (класс, оценка, местоположение, размер).

### Метрики YOLOv5

<image src="./images/YOLOv5_metrics.png"></image>

### Сравнение показателей YOLOv5 и YOLOv7 на тестовом датасете

| YOLOv5 | YOLOv7 |
| --- | --- |
| <image src="./images/y5/confusion_matrix.png"></image> | <image src="./images/y7/confusion_matrix.png"></image> |
| <image src="./images/y5/f1curve.png"></image> | <image src="./images/y7/F1_curve.png"></image> |
| <image src="./images/y5/P_curve.png"></image> | <image src="./images/y7/P_curve.png"></image> |
| <image src="./images/y5/PR_curve.png"></image> | <image src="./images/y7/PR_curve.png"></image> |
| <image src="./images/y5/R_curve.png"></image> | <image src="./images/y7/R_curve.png"></image> |  

### Оценка производительности моделей
