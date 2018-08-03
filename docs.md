# Вызов нативных функций
У нативных функций следующая сигнатура: `fn(&AMX, *mut Cell)`, где `*mut Cell` массив параметров. Первый (нулевой) элемент массива - количество аргументов, все последующие непосредственно аргументы.

Список аргументов:
* Примитив.
* Указатель на примитив.
* Массив.
* Строка.

Все они являются `Cell`, все, кроме примитива, является указателем.

Аргументы идут в прямом порядке.

> Интересная особенность: нативная функция отсутствует, пока она не задействуется в гейммоде.