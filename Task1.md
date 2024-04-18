# Задание 1: Главное меню!

## Описание

Каждая команда делает свою игру. Это может быть что угодно от кликера, до хоррор шутера. Но есть две механики, которые могут присутствовать в любой игре независимо от жанра, сеттинга и сюжета. Сегодня мы попробуем реализовать эти две механики. В этом задании мы сделаем главное меню. Наше меню будет довольно базовым, вы сможете улучшить его и дополнить при необходимости. Мы создадим кнопку начала игры и кнопку выхода. И так же добавим кнопку глобального включения и выключения звука.

<img src="https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/img/Task1.gif" width="600"/>

## Инструкция

Создай сцену для главного меню.

Создай в сцене канвас и не забудь настроить его canvas scaler комопнент

<img src="https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/img/canvas_scaler.png" width="400"/>

Создай две кнопки и расположи их по центру экрана, друг под другом.

<img src="https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/img/main_menu.png" width="400"/>

Создай еще одну кнопку в угул экрана. Удали у нее текстовую составляющую, спрайт кнопки замени на иконку звука. Можешь поискать ее в интернете или взять наш вариант.

[Иконка SoundOn](https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/img/SoundOn.png)

[Иконка SoundOff](https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/img/SoundOff.png)

<img src="https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/img/sound_button.png" width="400"/>

Создай в сцене пустой объект, назови его MenuManager. Этот объект будет нашим хранителем скриптов для главного меню.

Создай два скрипта [MainMenu](https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/scripts/MainMenu.cs) и [SoundToggle](https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/scripts/SoundToggle.cs)

Скопируй содержимое скриптов и замени "???" на недостающие фрагменты кода.

Добавь оба скрипта в компоненты к объекту MenuManager и не забудь навесить ссылки на спрайты иконок звука и кнопку звука.

<img src="https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/img/MainMenu_components.png" width="400"/>

На саму кнопку звука навесь в обработчик OnClick ссылку на скрипт **SoundToggle** и укажи метод **SoundToggleButton()**

<img src="https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/img/SoundButton_OnClick.png" width="400"/>

Чтобы проверить кнопку звука в игре, добавь в проект фоновую мелодию. Создай в сцене объект с AudioSource, навесь ссылку на звуковой файл и поставь галочки в PlayOnAwake и Loop.

<img src="https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/img/background_sound.png" width="400"/>

Аналогично навесь обработчики на кнопки Начать игру и Выход. Методы называются **GameStartButton()** и **GameExitButton()**

Остался последний шаг. Создай новую сцену для основной игры, можешь назвать ее Main или Level1. Открой Build Settings и добавь обе сцены в окно настроек билда.

<img src="https://github.com/copetonrob/YP_Unity_M4_W5/blob/main/img/build_settings.png" width="600"/>

Запусти проект и проверь, что все работает.
