# Программа для оценки скорости выполнения алгоритма простого скользящего среднего

## Описание
Эта программа написана на QT и предназначена для оценки скорости выполнения алгоритма простого скользящего среднего.

## Основные функции программы
### sempleMovingAvrage

template <typename T> QVector<T> MainWindow::sempleMovingAvrage(const QVector <T>& data, int period)
Данная функция вычисляет скользящее среднее для заданного вектора данных data и заданного периода period. Возвращает вектор с результатами.

### sempleMovingAvrageOnce

template <typename T> T MainWindow::sempleMovingAvrageOnce(const QVector <T>& data, int period)
Данная функция вычисляет скользящее среднее для заданного вектора данных data и заданного периода period. Возвращает результат однократного вычисления.

### measurePerfomance

void MainWindow::measurePerfomance()
Эта функция измеряет производительность алгоритма скользящего среднего для разных размеров окна. Выводит результаты в виде времени выполнения в миллисекундах для последовательности значений типа float и double.

### measurePerfomanceOnce

void MainWindow::measurePerfomanceOnce(int fl)
Эта функция измеряет производительность алгоритма скользящего среднего для разных размеров окна. Выводит результаты в виде времени выполнения в наносекундах для последовательности значений типа float (если fl=0) или double (если fl=1).

## Использование программы
1. Запустите программу через QT.
2. Нажмите кнопку "Сгенерировать последовательность" для получения случайной последовательности длинны 1000000 (последовательность вы не увидите т.к задача в этом не стояла).
3. Выберите одну из следующих опций:
   - Нажмите кнопку "Измерить производительность" для оценки производительности алгоритма для разных размеров окна для последовательности значений типа float и double .
   - Нажмите кнопку "Измерить производительность за одно окно float " для получения статистики длительнасти работы алгоритма (вывод производится в формате (Длинна окна_время в наносекундах)).
   - Нажмите кнопку "Измерить производительность за одно окно double " для получения статистики длительнасти работы алгоритма (вывод производится в формате (Длинна окна_время в наносекундах)).
4. Результаты измерений производительности будут отображены в текстовом поле.
## Примеры визуализации
![image](https://github.com/Akapulka00/-/assets/91537466/78ca49f0-a53e-450f-bc48-1954afca07cf)

## Использование
1. Откройте программу.
2. Нажмите кнопку сгенерировать случайную последовательность.
3. Выбирите режим работы.
4. Подождите отображения статистики.
5. Скопируйте данные и закройте программу.

