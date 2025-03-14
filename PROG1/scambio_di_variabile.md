# Scambio di variabili

Il confronto e lo scambio di variabili sono alla base degli algoritmi di ordinamento come il bubblesort

Per fare lo scambio ci va sempre una variaible d'appoggio temporanea

```c
int x = 5;
int y = 2;
int temp = 0;
temp = x;
x = y;
y = temp;
```