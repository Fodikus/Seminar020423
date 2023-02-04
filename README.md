# Seminar020423
Домашняя работа №3 к семинару "Знакомство с языками программирования"

# Задача 19: Напишите программу, которая принимает на вход пятизначное число и проверяет, является ли оно палиндромом.
```
Console.Write("Введите число: ");
int n = Convert.ToInt32(Console.ReadLine());
string s = Convert.ToString(n);
while (s.Length!=5)
{
    Console.Write($"Вы ошиблись! {s.Length}\nВведите пятизначное число: ");
    n = Convert.ToInt32(Console.ReadLine());
    s = Convert.ToString(n);
}

if ((s[0] == s[4]) & (s[1] == s[3]))
    Console.WriteLine($"Число {n} -> палиндром");
else
    Console.WriteLine($"Число {n} -> не палиндром");
```

# Задача 21: Напишите программу, которая принимает на вход координаты двух точек и находит расстояние между ними в 3D пространстве.
```
Console.Clear();       
Console.Write("Введите координату x1: ");
double x1 = Convert.ToDouble(Console.ReadLine());
Console.Write("Введите координату y1: ");
double y1 = Convert.ToDouble(Console.ReadLine());
Console.Write("Введите координату z1: ");
double z1 = Convert.ToDouble(Console.ReadLine());
Console.Write("Введите координату x2: ");
double x2 = Convert.ToDouble(Console.ReadLine());
Console.Write("Введите координату y2: ");
double y2 = Convert.ToDouble(Console.ReadLine());
Console.Write("Введите координату z2: ");
double z2 = Convert.ToDouble(Console.ReadLine());

double s = Math.Sqrt(Math.Pow(x2 - x1, 2) + Math.Pow(y2 - y1, 2) + Math.Pow(z2 - z1, 2));
Console.WriteLine($"A({x1},{y1},{z1}); B({x2},{y2},{z2}), -> {Math.Round(s, 2)}");
```

# Задача 23: Напишите программу, которая принимает на вход число (N) и выдаёт таблицу кубов чисел от 1 до N.
```
Console.Clear();
Console.WriteLine("Введите число a: ");
int a = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("Введите число b: ");
int b = Convert.ToInt32(Console.ReadLine());

if (a > b)
    Console.WriteLine($"a={a}; b={b} -> max {a} ");
else
    Console.WriteLine($"a={a}; b={b} -> max {b} ");
```
