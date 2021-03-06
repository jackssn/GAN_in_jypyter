# GAN_in_jypyter

Домашнее задание на тему **CycleGAN**. Проект включает в себя:

1. Jypyter Notebook, содержащий Pipeline для обучения сети по основным 
датасетам в задачах CycleGAN, а именно:
    * apple2orange
    * cezanne2photo
    * horse2zebra
    * monet2photo
    * summer2winter_yosemite
    * ukiyoe2photo
    * vangogh2photo
2. Ссылку на скачивание собственного датасета с названием *overwatch2csgo*
3. Код для создания своего датасета из имеющихся видео
4. "Веса" для модели, обученной на датасете *apple2orange*

## Инструменты

1. Windows 10 (x64)
2. Nvidia CUDA (GeForce 1060 6Gb)
2. Python 3.7 (Anaconda3)
3. Modules:
    * requests                          2.22.0
    * torch                             1.4.0
    * torchsummary                      1.5.1
    * torchvision                       0.5.0
    * tensorboard                       2.2.2
    * numpy                             1.18.4
    * matplotlib                        3.1.1

## Как запустить

1. Скачать файл `project.ipynb`
2. Запускать последовательно ячейки. Все необходимые 
папки создадутся автоматически. Датасеты скачивать отдельно не нужно, 
внутри файла есть команды для сбора датасетов

## Ссылки

[[1]](https://github.com/hanyoseob/pytorch-CycleGAN) Проект, взятый за основу, упрощенный и перенесенный в Jypyter Notebook<br/>
[[2]](https://github.com/bendangnuksung/fortnite-pubg) Проект, который вдохновил на "перерисовку игр"<br/>
[[3]](https://jackssn.com/result/apple2orange/90epochs) Результат работы 
модели на датасете apple2orange после обучения на 90 эпохах<br/>
[[4]](https://jackssn.com/result/apple2orange/190epochs) Результат работы 
модели на датасете apple2orange после обучения на 190 эпохах<br/>
[[5]](https://jackssn.com/datasets/overwatch2csgo.zip) Ссылка на скачивание датасета overwatch2csgo<br/>
[[6]](https://jackssn.com/result/overwatch2csgo) Результат работы модели на "своем датасете" после обучения на 80 эпохах<br/>
[[7]](https://jackssn.com/weights/apple2orange/model_epoch0190.pth) Веса модели apple2orange после 190 эпох

## Вывод

Большой разницы в картинках на своем датасете нет. Вероятно, неправильно выбраны параметры при обучении или слишком маленький набор данных, так как в успешных кейсах было примерно по 40 тыс картинок для тренировки и тестирования.

Результат работы на стандартном датасете apple2orange также требует более тщательного подбора параметров и увеличения количества эпох обучения.

## Примечание

1. В среднем на 10 эпох при batch_size=5 и 200 итерациях на 1 эпоху тратится около 1 ч.
