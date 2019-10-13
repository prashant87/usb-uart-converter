# USB-UART преобразователь с гальванической изоляцией

Проект создан для безопасной отладки силовых преобразователей и иных устройств, работающих с высоким напряжением, через интерфейс UART с помощью функции *printf*. Для изоляции выбран цифровой изолятор от компании Texas Instruments - **ISO7721DR** с напряжением изоляции до 2500В. Основной для конвертера служит популярная микросхема **CP2102** от компании Silabs. 

Преобразователь может работать с микроконтроллерами, и иными устройствами, с логическим уровнем 3.3В (например, STM32 и прочие) и 5В (например, ATmega), что делает его универсальным. Выравнивание уровней осуществляется с помощью подачи напряжения с основной платы на преобразователь (вывод VREF).

![3D вид платы](https://habrastorage.org/webt/rk/n7/86/rkn786vsd8srrjz3-s0azatiqno.png)

# Технические характеристики

* Тип преобразователя: *USB -> UART*
* Преобразователь: *CP2102*
* Гальваническая изоляция: *Да*
* Напряжение изоляции: *2500 В*
* Логические уровни: *2.5, 3.3 и 5В*
* Температурный диапазон: *-40...+85°С*

# Структура проекта

* Hardware
    * AltiumProject - исходный проект в AD19
    * Documents - принципиальная схема в формате PDF и спецификация (BOM)
    * Manufacture - набор файлов для производства печатной платы (Gerber и NC Drill)
    * Mechanical - 3D модель устройства

# Лицензирование

Все исходные материалы для проекта распространяются по лицензии [MIT](./LICENSE "Описание лицензии"). Вы можете использовать проект в любом виде, в том числе и для коммерческой деятельности, но стоит помнить, что автор проекта не дает никаких гарантий на работоспособность устройства или частей проекта, а так же не несет никакой ответственности по искам или за нанесенный ущерб.

# Контакты

* E-mail: *ilya@nordic-energy.org*
* Telegram: [*@aiki01*](https://t.me/aiki01 "Чат в телеграмме")
