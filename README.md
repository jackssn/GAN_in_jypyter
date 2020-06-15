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
[[3]](https://jackssn.com/result/apple2orange) Результат работы 
модели на датасете apple2orange после 
обучения на 90 эпохах<br/>
[[4]](https://jackssn.com/datasets/overwatch2csgo.zip) Ссылка на скачивание датасета overwatch2csgo<br/>
[[5]](https://jackssn.com/result/overwatch2csgo) Ссылка на результат работы модели на "своем датасете"

## Примечание

1. Нужно попробовать "дообучить" модели на большем количестве эпох 
и на других датасетах. В среднем на 10 эпох тратится около 1 ч.
