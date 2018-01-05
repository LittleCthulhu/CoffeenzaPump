# CoffeenzaDroid
Управляющее Android-приложение для кофейного поддона.

# Архитектура решения

## [Поддон - Tray](https://github.com/LittleCthulhu/CoffeenzaTray)
* Прошивка для Arduino
* Собирает статистику с NFC меток на кружках

## [Приложение - Pump](https://github.com/LittleCthulhu/CoffeenzaPump)
* Android приложение на Xamarin (C# + Visual Studio 2017)
* Забирает статистику с поддона и отправляет её на сервер
* Управляет списком пользователей
* Визуализирует статистику с использованием отметок во времени (milestone'ов)

## [Сервер - Storage](https://github.com/LittleCthulhu/CoffeenzaStorage)
* В основе - база данных
* Хранит статистику, умеет отдавать её приложению
