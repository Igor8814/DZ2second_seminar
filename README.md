1. Напишите программу, которая принимает
 на вход вещественное число и показывает сумму его цифр.
 Пример:
 - 6782 -> 23
 - 0,56 -> 11
~~~
real_number = input('Введите вещественное число: ')
sum = 0
for i in real_number:
    if i != '.':
        sum += int(i)
print(sum)
~~~
2. Напишите программу, которая принимает
 на вход число N и выдает набор произведений чисел от 1 до N.
 Пример:
- пусть N = 4, тогда [ 1, 2, 6, 24 ] (1, 1 * 2, 1 * 2 * 3, 1 * 2 * 3 * 4)
~~~
n = int(input('Введите число: '))
product_numbers = 1
for i in range(1, n + 1):
    product_numbers *= i
    print(product_numbers, end =' ')
 ~~~
 3. Задайте список из n чисел последовательности
 $(1+ 1 /n)^n$ и выведите на экран их сумму.
~~~        
n = int(input('Введите число: '))
spisok = [] 

for i in range(1, n + 1):
    spisok.append((1 + 1/i)*i)
print(spisok)    
print(int(sum(spisok)))
~~~
4. Реализуйте алгоритм перемешивания списка.
~~~
import random
list = ['a', 'b', 'c', 'd', 'e']
print(list)
random.shuffle(list)
print(list)
~~~     