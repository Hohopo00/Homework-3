# Домашнее задание к работе 3



## Условие задачи
Написать и отладить программу вычисления расстояния между двумя точками, заданными координатами x и y. 

## 1. Алгоритм и блок-схема

### Алгоритм
1. **Начало**
2. Задать исходные данные:
   - `x1` — Координата х первой точки
   - `y1` — Координата у первой точки
   - `x2` - Координата х второй точки
   - `y2` - Координата у второй точки
   - `distance` - Расстояние
3. Разница между координатами х:
   - `double dx = x2-x1`
4. Разница между координатами у:
   - `double y2 = y2-y1`
4. Вычисление расстояния по теореме Пифагора:
   -` distance = sqrt(dx*dx+dy*dy)`
5. Вывести результаты расчетов с подстановкой всех значений в текст.
6. **Конец**

### Блок-схема 
<img width="2404" height="4244" alt="image" src="https://github.com/user-attachments/assets/9f24613d-605f-4178-bf3e-20a4d4b4ed11" />
https://app.diagrams.net/?src=about&splash=0#R7ZZNj5swEIZ/DVJ76CpA2KTHhbR7yUqrplLPE3BgFONBxlmS/fUdg1OUhKjRJu0pEkiedz5sz2MLvDApt88aquKFMiG98JsXJprIdKNymwgpvWCEmRfOvCAY8esF3894/dY7qkALZS5JCLqEN5Ab0SkxqPVTmtKGC7S+2uyk89UNlhIUW/GKlFk4j882SMwVj1OeWGgW3oQ2mIJ8cg5DFatpgTKbw442dnm1gXS9t+KCNL5zWZCuJru1WeC7nSN8fJgexCxsLjtGrGpRc9Trftf+kfQC24PAOdTGCSlJCVWNy3YjVilB56hiMoZKJ7ke8YbE9myfW8k1+VlQKYzecYhLmHYJuwOrwcwUjkMw6bRCYF7sS351eKDuhPxP3R4pDxzVYcLhCWEviBdGo8pZpkYxrWPOvE/T9l/TWiQkiYHOFHXgUcojac9eipU5S76uIOU5523MbNwrP9yGrUScu5LUsFlglgllmZEBAz2gilCZtiFRzA+f72T0EHkRLzxh2+9tfmy4Ngkp3gtgy0ow/UbYE3AZ2GAYrEMZTi5juY+7BuV4CGWM+UykWIKNXAJfz1TcgX4c6GT8/4BGJ6AktgA6UL/cEvwPUSq531L0WH5aarMv/gm68BRdOIBJwlLIV6rRINn6uos9wvc3QodHEFUhNN6InO+PLkM3vZ7c49BVzERl2/MJSvv1/Hy/hdewvPAbeYtrOBmC2aApMg0NyDvPG/CMon/Gk83+h7n1HfxP/wY=#%7B%22pageId%22%3A%22_6kMP9uhorh4GVad86cH%22%7D



## 2. Реализация программы

```
#define _CRT_SECURE_NO_WARNINGS  
#include <stdio.h>               
#include <math.h>                
#include <locale.h>              

int main() {                     
    setlocale(LC_ALL, "RUS");  

    double x1, y1, x2, y2, distance;   // Объявляем переменные для координат точек и расстояния
                                 

    // Ввод данных пользователя
    printf("Введите координаты первой точки:\n");  //Введение координат первой точки
    printf("x1: ");                       
    scanf("%lf", &x1);                    
                                         
    printf("y1: ");                      
    scanf("%lf", &y1);                   

  
    printf("Введите координаты второй точки:\n");   // Введение координат второй точки
    printf("x2: ");                       // Подсказка для ввода x2
    scanf("%lf", &x2);                    // Чтение числа типа double в переменную x2
    printf("y2: ");                       // Подсказка для ввода y2
    scanf("%lf", &y2);                    // Чтение числа типа double в переменную y2

    // Расчет расстояния между точками
    double dx = x2 - x1;                  // Вычисляем разность по оси X
    double dy = y2 - y1;                  // Вычисляем разность по оси Y
    distance = sqrt(dx * dx + dy * dy);   // Вычисляем расстояние по теореме Пифагора:
                                        

    // Вывод результата
    printf("Расстояние между точками: %.2f\n", distance);  

    return 0;                            // Завершение программы 
```

## 3. Результаты работы программы

```
Введите координаты первой точки:
x1: 7
y1: 9
Введите координаты второй точки:
x2: 8
y2: 0
Расстояние между точками: 9,06
```

## 4. Информация о разработчике

Прохорова Виктория, бТИИ-251

