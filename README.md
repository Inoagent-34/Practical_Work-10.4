  Практическая работа 10.4
  Задание: Необходимо решить задачу Практической работы 9.5, заменив отдельные функции кода при их вызове на команды с помощью директив, а аргументы — с помощью заменяемых параметров. Объедините две предыдущие задачи в один код с возможностью компиляции задачи по очереди, используя директивы условной компиляции и выбора компиляции в начале программы.
  Решение (программа Task_1)
  При помощи директив #define созданы макросы, заменяющие в тексте программы вызовы функций: FIB_COUNT заменяет вызов процедуры Calculation(n), GAMING - вызов Game(), RENDERING -  вызов  View(Rendered_Chart), END - заменяет оператор return 0. 
  Макросы GAME_1, GAME_2, GAME_3 определяют содержимое массива Data_Chart, которое можно менять в тексте программы, меняя, таким образом, загаданные символы в игре.
    В программе предусмотрена выборочная компиляция путём выбора участков кода. Для этого директивой define определен объект MODE, в завимости от значения которого выбираются участки кода, подлежащего компиляции. Объект MODE может принимать значения FIBONACHHI и GAME, определенные как 0 и 1. 
    Внутри кода установлены участки, подлежащие выборочной компиляции, при помощи директив #if, #else и #endif. Таким образом, в зависимости от установленного объектом MODE, программа компилируется либо на вычисление чисел Фибоначчи, либо для игры по отгадыванию символов.
  Сам код устроен так же, как и в заданиях Практической работы 9.5.
