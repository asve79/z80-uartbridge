# z80-uartbridge
Мост для трансляции UART&lt;->ZIFI на TS-CONF

# Зачем?
В процессе разработки я ушатал Zifi модуль подключаемый к PC. Писать эмуляттор команд долго, плюс нужно отлаживаться, смотреть на поведение живого модуля, которого нет. Пока жду прихода модулей, которые могут ехать больше месяца, нужно на чем-то работать.
Собственно есть ева с модулем, который на PC не работает но работает на еве. Значит можно использовать его.

# Как работает?
Подключаем еву в конфигурации ts-conf к порту PC, запускаем мост.
PC пишет в порт. Ева его получает, транслирует на Zifi, ответ транслирует обратно.
Да, работает медленней. Но цель проекта обеспечить работу с Zifi и понимать что проходит сквозь порты.
Вопрос перфоманса пока не стоит.
Видно какие данные проходят сквозь порты.

# Релизы
Готов релиз 1.0
