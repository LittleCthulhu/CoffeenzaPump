# CoffeenzaPump
Управляющее Android-приложение для кофейного поддона. Центральное звено эко-системы Coffeenza.

# Архитектура решения
## [Поддон - Tray](https://github.com/LittleCthulhu/CoffeenzaTray)
* [Прошивка для Arduino](https://github.com/Be3yH4uK/SmartCoffeeMachine) авторства @Be3yH4uK
* Собирает статистику с NFC меток на кружках

## [Приложение - Pump](https://github.com/LittleCthulhu/CoffeenzaPump)
* Android приложение на Xamarin.NET
* Забирает статистику с поддона и отправляет её на сервер
* Управляет списком пользователей
* Визуализирует статистику с использованием отметок во времени (milestone'ов)

## [Сервер - Store](https://github.com/LittleCthulhu/CoffeenzaStore)
* База данных
* Хранит статистику, умеет отдавать её приложению
