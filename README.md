## ImageCaptioning

Создание подписей к изображениям с помощью рекуррентных нейронных сетей. <br>
Принцип работы таков:
- Изображение векторизуется с помощью VGG-19 (предобученной на ImageNet)
- Полученные эмбеддинги используются внутри LSTM + Attention сети

Как получается "визуалцизация внимания": 
- Запоминаются активации нейросети на разных слоях её вывода. 
- По ним строятся grayscale маски
- Накладываем маску на изображение

Несколько примеров работы:

![alt text](https://github.com/IlidanNaga/ImageCaptioning/blob/main/Results/eg1.png?raw=true)
![alt text](https://github.com/IlidanNaga/ImageCaptioning/blob/main/Results/eg2.png?raw=true)
![alt text](https://github.com/IlidanNaga/ImageCaptioning/blob/main/Results/eg3.png?raw=true)
