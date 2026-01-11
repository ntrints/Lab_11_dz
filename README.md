# Lab_11_dz
Домашняя работа к лабораторной работе №11

# Условия задачи
Количество элементов массива, значения которых больше заданного числа A.

# Блок-схема
<img width="452" height="1692" alt="flowchart_1768166555550" src="https://github.com/user-attachments/assets/437cfba8-53d4-4211-8049-700f7071825e" />

# Реализация программы

```
#include <stdio.h>
#include <locale.h>
#define MAX 100   

int main() {
    setlocale(LC_ALL, "RUS");

    int n;
    int c = 0;
    int arr[MAX];

    puts("Введите количество элементов массива");
    scanf("%d", &n);

    if (n > MAX || n <= 0) {
        puts("Некорректное количество элементов");
        return 1;
    }

    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] > 10 && i % 2 == 0) {
            c++;
        }
    }

    printf("Количество элементов: %d\n", c);

    return 0;
}
```
<img width="891" height="284" alt="image" src="https://github.com/user-attachments/assets/71b0b884-7837-4723-8da2-bf5327036a89" />
