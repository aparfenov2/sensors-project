
# План работ по проекту Flutter Sensors
nn| Описание | К-во часов
-|-|-
1| Реализация окон (визуальная часть)|153
1.1| Main Page | 62
-| Гугл карта с метками| 25
-| [Таблица справа](#user-content-таблица-справа) | 37
1.2| [Account Window](#user-content-account-window) | 18
1.3| [Details Window](#user-content-details-window) | 73
-|[Виджет текущего состояния](#user-content-виджет-текущего-состояния)|16
-|[График истории](#user-content-график-истории)|29
-|[Consumption](#user-content-consumption)|8
-|[Таблица истории](#user-content-таблица-истории)|8
-|[General Settings Window](#user-content-general-settings-window)|12
2| Подключение к источнику данных
-|  создание тестового аккаунта
-|  запрос данных при отображении
-|  сохранение данных при изменениях
3 | остальное
-| тестирование
-| публикация в Google Play

## Анализ web-версии проекта

## 1. Общее

Описание | К-во часов
-|-
навигация| 2

## 2. Main Page

https://fuelowl.engix.ie/dashboard/3f1f49e0-51e1-11ed-86fe-9dcd4c516023

![Main Page](images/image.png)

Описание | К-во часов
-|-
*App bar*|2
-навигация
-кнопка Назад,
-кнопка Домой
-кнопка Logout
-Contact Us (mailto:support@woodco-energy.com)
-Account [Account Window](#user-content-account-window)
*плавающий логотип внизу*|1
![logo](images/image-24.png)
*Гугл карта с метками*
![Google Map](images/image-8.png)
поиск и выбор виджета|2
рисование|2
подключение к источнику данных|2
общая логика|1
тестирование|1
pan, zoom | 1
full screen | 1
обновление таблицы при pan/zoom | 2
*Сlick Baloon - Show Plant Information*
![Baloon Details Wnd](images/image-17.png)
рисование|2
подключение к источнику данных (чтение, сохранение)|2
тестирование|1
*Baloon Popup*
![Baloon Popup Wnd](images/image-18.png)
рисование|2
подключение к источнику данных (чтение, сохранение)|2
тестирование|1
**Всего** | 25

### Таблица справа
![Right Summary Table](images/image-9.png)

Описание | К-во часов
-|-
поиск и выбор виджета|2
рисование таблицы| 2
подключение к источнику данных|2
общая логика|1
тестирование|1
сортировка|1
paging|1
scrolling|1
*окно Add Owner*
![Add Owner Wnd](images/image-10.png)
рисование|2
подключение к источнику данных (чтение, сохранение)|2
*окно Add Plant*
![Add Plant Wnd](images/image-11.png)
рисование|2
подключение к источнику данных (чтение, сохранение)|2
*окно Add Silo*
![New Silo Wnd](images/image-12.png)
рисование|2
подключение к источнику данных (чтение, сохранение)|2
*Search Box*
![Search Widget](images/image-13.png)
рисование|1
подключение к источнику данных (чтение)|1
*click details icon - Show Plant Information*|1
![Show Plat Info Wnd](images/image-14.png)
*Gate Token Wnd*|2
![Gate Token Wnd](images/image-15.png)
*Edit Plant Info*
![Edit Plant Info Wnd](images/image-16.png)
рисование|2
подключение к источнику данных (чтение)|2
*Delete Plant Btn*
*Delete Silo*
*кастомные виджеты состояния (отрисовка)*
Online|1
Level, %|1
Mass, t|1
Owner (3 rows)|1
*кастомные виджеты состояния (подкл. к данным)*|2
*click row - open Details Window*
[Details Window](#user-content-details-window)
**Всего** | 37

## Account Window
Описание | К-во часов
-|-
*Profile*
![Profile](images/image-1.png)
![Profile-bottom](images/image-2.png)
рисование|2
подключение к данным|2
*Security*
![Security Window](images/image-3.png)
рисование|2
подключение к данным|2
*Notification Settings*
![Notification Settings Window](images/image-4.png)
![Notif2](images/image-5.png)
рисование|2
подключение к данным|2
*Режим полного экрана*|1
*Инфа о текущем пользователе в AppBar*|1
![Full Screen](images/image-6.png)
*Окно уведомлений*
![Notif Wnd](images/image-7.png)
рисование|2
подключение к данным|2
**Всего** | 18

## Details Window
![Details Window](images/image-19.png)

### Виджет текущего состояния
![current state wnd](images/image-20.png)
Описание | К-во часов
-|-
рисование|2
подключение к данным|2
кнопка Show More Information изменяет отображение текущего виджета|1
кнопка General Settings открывает окно [General Settings Window](#user-content-general-settings-window)|1
*кастомные иконки с данными*
рисование
LoRa|0.5
Battery|0.5
Env.Temp|0.5
Env.Humidity|0.5
Latest Data Timestamp|0.5
Signal Quality|0.5
WiFi|0.5
Angle.Y|0.5
Angle.X|0.5
Cleaning Cycles|0.5
Received Packages|0.5
подключение к данным|2
**Всего** | 16

### График истории
![history wnd](images/image-21.png)
Описание | К-во часов
-|-
поиск и выбор виджета|2
всплывающая метка|2
![popup value](images/image-34.png)
выделение и zoom|2
кнопка настроек Edit timewindow|1
![Alt text](images/image-35.png)
-открывает окно  Edit timewindow
*Realtime (окно настроек)*
![Edit timewindow - realtime](images/image-36.png)
рисование|2
подключение к данным|2
-возможность задать интервал
![realtime - interval](images/image-37.png)
-вкладка History
![chart - hsitory](images/image-38.png)
рисование|2
подключение к данным|2
-установка дат интервала через календарь|2
![hist-calendar](images/image-39.png)
-установка времени интервала через часы|2
![hist-clock](images/image-40.png)
-при нажатии на иконку E отображается *окно с табличными данными истории*
![realtime table data](images/image-41.png)
рисование|2
подключение к данным|2
-scrolling
-paging
*кнопка Distance Chart отображает окно Distance Chart*
![distance chart](images/image-42.png)
рисование|2
подключение к данным|2
-кнопка расширения на весь экран для любого из графиков|1
**Всего** | 29

### Consumption
Описание | К-во часов
-|-
![consumtion wnd](images/image-22.png)
рисование|2
подключение к данным|2
кнопка настроек отображает окно Estimation Period Settings
![estimation period settings](images/image-43.png)
рисование|2
подключение к данным|2
**Всего** | 8

### Таблица истории
Описание | К-во часов
-|-
![history table](images/image-23.png)
рисование|2
подключение к данным|2
-scrolling
-paging
кнопка Edit timewindow аналогично кнопке на графике, но с дополнениями
![history-timewindow-settings](images/image-44.png)
![history-timewindow-settings-2](images/image-45.png)
рисование|2
подключение к данным|2
**Всего** | 8

## General Settings Window
Описание | К-во часов
-|-
-scrollable
![genral settings](images/image-25.png)
рисование|2
подключение к данным|2
![alaram settings](images/image-26.png)
рисование|2
подключение к данным|2
![ui settings](images/image-27.png)
рисование|2
подключение к данным|2
*Silo calibration settings - level*
![Silo calibration settings - level](images/image-28.png)
*Silo calibration settings - mass*
![calib settings - mass](images/image-29.png)
рисование|2
подключение к данным|2
*Silo Alarm Settings*
![Silo Alarm Settings](images/image-30.png)
![alarm settings bottom](images/image-31.png)
рисование|2
подключение к данным|2
*Sensor Settings*
![Sensor Advanced Settings](images/image-32.png)
![Sensor Service Mode](images/image-33.png)
рисование|2
подключение к данным|2
**Всего** | 12
