﻿## Заключение
В данной статье предложен алгоритм расчета характеристик музыкального произведения с использованием метода главных компонент. Для оптимизирования алгоритма по скорости работы предложено обрабатывать 10-секундные сегменты мелодий отдельно. Так как в методе главных компонент используется перемножение матриц, то использование аудиозаписей небольшой длительности позволяет алогритму работать быстро. Недостатками предложенного подхода является необходимость наличия состоящей из разнообразных мелодий обучающей базы, а также необходимость привлечения эксперта для выявления того, каким реальным характеристикам (жанру, темпу и т.п.) соответствуют выбранные главные компоненты. Дальнейшим направлением исследований может быть разработка алгоритма. позволяющего обрабатывать мелодии разных длительностей, а также рассмотрение возможности использование вейвлетов в дополнение к оконному преобразованию Фурье для повышения точности расчета амплитудно-частотной характеристики.

