## SneakerShazam
Увидел классные кроссовки на ком-то на улице, хочешь такие же, но боишься подойти и спросить бренд и название модели? Отправь фотографию обуви боту и узнай ответ. На текущий момент бот обучен на 20 видах кроссовок (Nike, Adidas, Reebok, Air Jordan)
Бот работает на 2 моделях: YoloV4 и ResNet101V2
Наша первая модель (YoloV4) детектирует кроссовки на фотографии, рисуя вокруг них bounding box. YoloV4 была обучена на 1000 фотографий

![detectioon](data/images/input/sneaker_132032976_342.jpg)

Затем по координатам bounding box'а мы обрезаем фотографию и в таком виде передаем второй модели - ResNet101V2.
![cropped](data/images/output/photo_132032976_342.jpg)


Вторая модель (ResNet101V2) нужна для классификации модели кроссовка. ResNet101V2 была обучена на 4000 фотографии 20 классов.

Проект был выполнен за 10 дней при участии:
- https://github.com/jabulani9955
- https://github.com/DaRealMumba
- https://github.com/Damotsoff

## Ссылка на бота
- https://t.me/Bashmak_shazam_bot
