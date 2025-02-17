### Фактические результаты:

Научно-исследовательская работа производится в рамках проекта по разработке веб-сервиса по поиску подобной музыки.

* В настоящее время сформулирована тема научно-исследовательской работы – «Создание web-сервиса для поиска музыки по подобию», а также выбраны: язык программирования Python 3, фреймфорк Django и вспомогательная библиотека для обработки музыки LibRosa.
* Параметры музыкальной композиции будут рассчитываться с использованием быстрого преобразования Фурье (БПФ), на данный момент реализован расчет темпа музыки.
* Ввиду того, что музыкальные композиции содержат в себе большое множество вычисляемых характеристик, требуется обеспечить сервису возможность выполнять их расчёт в асинхронном режиме в соответствии с очередью задач. В качестве подзадачи также необходимо по имеющимся в открытом доступе материалам изучить возможные методы расчета музыкальных характеристик с использованием БПФ и оптимизировать алгоритмы таким образом, чтобы обеспечить высокую скорость расчета.
* Кроме того, ввиду субъективности выражения «подобная музыка», предполагается, что пользователь сможет самостоятельно регулировать, какие параметры для него больше определяют «подобие» (темп, жанр, наличие вокала обычно более понятны для человека без музыкального образования, чем гармония или главная нота в музыке) и при этом существенно влиять на итоговый результат поиска.
* Пользователю должна быть представлена рекомендательная система, осущесвляющую отбор подобной музыки в первую очередь - на основе контента, по возможности - с использование коллаборативной фильтрации, то есть результатов поисков других пользователей.
