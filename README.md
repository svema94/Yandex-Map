# Тестирование Яндекс Маршрутов

♻️ Яндекс Маршруты — сервис, который строит маршруты для транспорта разных видов, рассчитывает время и стоимость поездки.

# 1. Тестирование валидации полей в форме
В требованиях к Яндекс Маршрутам есть таблица с ограничениями на ввод в поля формы. 
https://code.s3.yandex.net/qa/schemes/sprint01-project-002.png
Валидация формы работает следующим образом: в случае корректного ввода появляется расчёт времени и стоимости поездки. В случае некорректного ввода появляется сообщение об ошибке. 
Необходимо проверить, что в реализации применены все требования к полям и валидация проходит так, как задумано.

💡 Обратить внимание! В поля «Откуда» и «Куда» можно вводить только ограниченное количество адресов из таблицы в требованиях: Усачева, 3; Комсомольский проспект, 18; Зубовский бульвар, 37; М. Пироговская, 25; Хамовнический Вал, 34; Фрунзенская набережная, 46; 3-я Фрунзенская улица, 12. 
Используй перечисленные адреса в качестве тестовых данных в таблицах классов эквивалентности и граничных значений, а затем и в тест-кейсах.

В рамках задания нужно:
Провести тест-анализ требований на валидацию полей.
Создать набор тест-кейсов на проверку валидации полей формы Яндекс Маршрутов. Применить техники тест-дизайна: классы эквивалентности и граничные значения.
Протестировать валидацию полей и завести баг-репорты.

# 2. Тестирование расчета стоимости и времени поездки на собственном автомобиле

Яндекс Маршруты рассчитывают время и стоимость поездки, в том числе на своем автомобиле. В требованиях есть таблицы средней скорости автомобиля и расстояний между адресами, на основе которых должен производиться расчет времени поездки. По стоимости указано, что за 1 км. расход составляет 20 руб.
https://code.s3.yandex.net/qa/schemes/sprint01-project-005.png,
https://code.s3.yandex.net/qa/schemes/sprint01-project-006.png
Необходимо проверить, что приложение верно рассчитывает время и стоимость поездки для собственного автомобиля.

 ⚙ Время поездки рассчитывается по формуле t = S/V (где t - время поездки, S - расстояние, V - средняя скорость);
 Стоимость поездки рассчитывается по формуле: *Р (итоговая) = S * P (где Р (итоговая) - стоимость поездки, S - расстояние, Р - стоимость 1 км.);*
 Важно! Средняя скорость для расчета берется по времени начала поездки.

В рамках задания нужно:
Провести тест-анализ требований расчёта времени и стоимости маршрута на собственном автомобиле. 
Применить технику тест-дизайна «Классы эквивалентности» и создать набор тест-кейсов на проверку правильности расчета времени и стоимости поездки на собственном автомобиле.
💡 При составлении тест-кейсов использовать значения только из колонки «Тестовые данные внутри класса»
Протестировать расчеты и завести баг-репорты

Требования на валидацию полей к Яндекс Маршрутам https://docs.google.com/document/d/1tleRVoK3off9RI6paLStjcCaRx9lWstOEIZtArhnLYI/edit?tab=t.0#heading=h.7j2fbty8r7vb

 Сылка на гугл-таблицу: https://docs.google.com/spreadsheets/d/1KuH7my235ADm3SpmezVSvl1ioAqFNm8DDqXgC1JyFyc/edit?usp=sharing
