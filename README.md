# Classification
Нахождение классификатора, который покажет лучшую полноту

Каналы онлайн-бронирования отелей сообщают, что значительное количество бронирований отменяется из-за аннулирований или неявки посетителей.
Для начала необходимо выполнить предобработку данных (#1).

Системе онлайн-бронирования требуются новые методики вычисления вероятности, что бронь будет отменена. Ваша цель - найти тот классификатор, который покажет лучшую оценку полноты и даст ответ на вопрос: из всех бронирований, которые были отменены, сколько система смогла найти? (#2)

Требуется создать функцию, которая примет на вход значение X и Y, которые были получены из предыдущей функции table_preprocessing.
1) Разделить полученные X и Y на тренировочную и тестовую выборки. Разделить выборку в соотношении 3 к 1.
2) Выбрать 3 классификатора и для каждого из них выполнить следующие шаги:
   — Импортировать классификатор из соответствующей библиотеки.
   — Создать объект классификатора.
   — Обучить классификатор с помощью метода fit.
   — Получить предсказания и записать их в переменную.
4) Оценить полноту каждого классификатора с помощью метода recall_score.
5) Функция должна вернуть строку "Имя_классификатора_1: полнота_для_классификатора_1. Имя_классификатора_2: полнота_для_классификатора_2. Имя_классификатора_3: полнота_для_классификатора_3."
6) Вызовите функцию hotel_booking_analyze с полученными из функции table_preprocessing значениями X и Y.
