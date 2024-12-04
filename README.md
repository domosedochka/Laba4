# Лабораторная работа №4.  Взаимодействие с сервером.
* Выполнила: Зинченко Анна
* Язык программирования: Java

# Что делает приложение?
Этот проект демонстрирует простой пример взаимодействия с сервером в Android-приложении. 
Чтобы запустить проект можно прочитать ["Как запустить"](#как-запустить)

# Функциональность:
* MainActivity: 
    Главный экран приложения содержит заголовок («Статистика проигрываемых песен») и кнопку «Просмотреть треки».  Нажатие на кнопку переводит пользователя на экран **TrackListActivity**.
<div align="left">
  <img src="https://github.com/domosedochka/Laba4/blob/main/Screenshot_2024-12-03-00-33-03-678_com.miui.videoplayer.jpg" width="200" />
</div>
* TrackListActivity: 
    Этот экран отображает список всех треков, добавленных в базу данных. Каждый трек представлен в виде строки, содержащей исполнителя, название и время добавления в список.
<div align="left">
  <img src="https://github.com/domosedochka/Laba4/blob/main/Screenshot_2024-12-03-00-33-08-083_com.miui.videoplayer.jpg" width="200" />
</div>
    После запуска приложение начинает асинхронно опрашивать внешний сервер с интервалом 20 секунд для получения информации о текущей воспроизводимой песне. В зависимости от полученных данных, приложение выводит соответствующее уведомление: 
    Если песня уже существует в базе данных:  отображается уведомление «Песня уже играет».
<div align="left">
  <img src="https://github.com/domosedochka/Laba4/blob/main/Screenshot_2024-12-03-00-33-21-963_com.miui.videoplayer.jpg" width="200" />
</div>
    Если песня новая и ее не существует в базе данных: отображается уведомление «Текущая песня».
<div align="left">
  <img src="https://github.com/domosedochka/Laba4/blob/main/Screenshot_2024-12-03-00-33-51-875_com.miui.videoplayer.jpg" width="200" />
</div>
    Затем песня добавляется в базу данных и отображается в списке треков на экране TrackListActivity.
<div align="left">
  <img src="https://github.com/domosedochka/Laba4/blob/main/Screenshot_2024-12-03-00-34-46-813_com.miui.videoplayer.jpg" width="200" />
</div>
   При отсутствии интернет-подключения приложение отображает уведомление об запуске в автономном режиме.
<div align="left">
  <img src="https://github.com/domosedochka/Laba4/blob/main/Screenshot_2024_12_04_13_02_42_903_com_example_laboratornaya4.jpg" width="200" />
</div>



# Как запустить
1. Загрузка или клонирование репозитория:
* Скачайте файлы проекта (ZIP-архив) и разархивируйте их в удобную папку или клонируйте репозиторий с помощью команды git clone [URL репозитория].

2. Открытие проекта в Android Studio:
* Откройте Android Studio.
* В главном окне выберите "Open an existing Android Studio project".
* Найдите папку, в которую вы скачали или клонировали проект, и выберите файл build.gradle.

3. Запуск приложения:
* В Android Studio, нажмите кнопку "Run" (зеленый треугольник) на панели инструментов.
* Выберите эмулятор или подключенное Android-устройство, на котором вы хотите запустить приложение.
* Дождитесь завершения сборки и запуска приложения.


