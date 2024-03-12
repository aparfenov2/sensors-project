
# План работ по проекту Flutter Sensors

1. Реализация окон (визуальная часть)
2. Подключение к источнику данных
    - создание тестового аккаунта
    - запрос данных при отображении
    - сохранение данных при изменениях

## Анализ web-версии проекта

1. Общее
    - навигация
        - кнопка Назад,
        - кнопка Домой

1. Main Page

https://fuelowl.engix.ie/dashboard/3f1f49e0-51e1-11ed-86fe-9dcd4c516023


![Main Page](images/image.png)

- App bar
    - навигация
        - кнопка Назад,
        - кнопка Домой
        - кнопка Logout
    - Contact Us (mailto:support@woodco-energy.com)
    - Account [Account Window](#user-content-account-window)
    - Режим полного экрана
        - почему-то только в Account Window
![Full Screen](images/image-6.png)
    - Окно уведомлений
        - почему-то только в Account Window
![Notif Wnd](images/image-7.png)

- Гугл карта с метками
![Google Map](images/image-8.png)
    - pan
    - zoom
    - full screen
    - обновление таблицы при pan/zoom
    - click Baloon
        - тоже что и Show Plant Information
![Baloon Details Wnd](images/image-17.png)
    - Baloon Popup
![Baloon Popup Wnd](images/image-18.png)

- Таблица справа
![Right Summary Table](images/image-9.png)
    - сортировка
    - paging
    - scrolling
        - реализуется стандартными средствами, 2h
    - Add Owner
![Add Owner Wnd](images/image-10.png)
    - Add Plant
![Add Plant Wnd](images/image-11.png)
    - Add Silo
![New Silo Wnd](images/image-12.png)
    - Search
![Search Widget](images/image-13.png)
    - click details icon:
        - Show Plant Information
![Show Plat Info Wnd](images/image-14.png)
            - Gate Token Wnd
![Gate Token Wnd](images/image-15.png)
            - Edit Plant Info
![Edit Plant Info Wnd](images/image-16.png)
            - Delete Plant Btn
        - Delete Silo
    - кастомные виджеты состояния
        - Online
        - Level, %
        - Mass, t
        - Owner (3 rows)
    - click row
    [Details Window](#user-content-details-window)

## Account Window

### Profile
![Profile](images/image-1.png)
![Profile-bottom](images/image-2.png)

### Security
![Security Window](images/image-3.png)

### Notification Settings
![Notification Settings Window](images/image-4.png)
![Notif2](images/image-5.png)

## Details Window
![Details Window](images/image-19.png)

TODO: Details Window
