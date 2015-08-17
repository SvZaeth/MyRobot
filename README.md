# MyRobot
Описание:

- Приложение является симулятором движения игрушечного робота по прямоугольному столу с размерами X x Y клеток.

Если размер не задан, задать размер 5х6 клеток.

- На столе больше нет никаких препятствий.

- Робот может свободно передвигаться по столу, но надо избежать его падения со стола. Любая комманда, которая может привести к падения робота со стола, должена быть предотвращена(пропущена), но любые последующие комманды, которые не приводят к падению робота, должны выполниться.

 

 

Техническая сторона:

- Создать приложение которое считывало комманды следующей формы:

PLACE X,Y,F

MOVE

LEFT

RIGHT

REPORT

 

- Размер стола задается при инициализации приложения

- PLACE задаст позицию робота на столе с координатами ячейки(X, Y) и сторону, в которую робот будет смотреть(F) - NORTH, SOUTH, EAST или WEST

- Ячейка с координатами 0,0 должна быть разценена как самый крайний юго-западный угол (SOUTH WEST)

- Самая первая валидная комманда для робота должна быть PLACE комманда. Приложение должно отклонить все комманды в последовательности пока комманда PLACE не будет выполнина

- MOVE - подвинет робота на одну ячейку вперед по направлению, которому он сейчас смотрит.

- LEFT и RIGHT - повернут робота на 90 градусов в соответствующем направлении без изменения его позиции

- REPORT - выведет текущие координаты робота (X, Y) и его текущее направление (F). Вывод может быть в произвольной форме.

 

- Робот, который не находится на столе, должен игнорировать комманды MOVE, LEFT, RIGHT и REPORT

- Ввод данных может быть как из файла так и из коммандной строки(на ваш выбор)

- Разработчик должен предоставить тестовые данные для проверки.

 

Ограничения:

- Робот не должен упасть со стола во время движения. Это так же включает себя начальное положение робота.

- Любая комманда, которая влечет за собой падение робота должна быть проигнорирована

 

Примеры Ввыода и Вывода:

а)

PLACE 0,0,NORTH

MOVE

REPORT

->Output: 0,1,NORTH

 

б)

PLACE 0,0,NORTH

LEFT

REPORT

->Output: 0,0,WEST

 

в)

PLACE 1,2,EAST

MOVE

MOVE

LEFT

MOVE

REPORT

->Output: 3,3,NORTH

 

Время на выполнение: 3 часа
