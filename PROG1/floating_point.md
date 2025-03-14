# Floating point

Secondo lo standard IEEE 754

# Divisione in C

In C per evitare errori di troncamento, le divisioni con la virgola vanno fatte con tutti tipi float.

Ad esempio:

```c
int x = 5;
int y = 2;
float res = x / y;  // Avrà valore 2.00
```
Invece è corretto:

```c
float x = 5;
float y = 2;
float res = x / y;  // Avrà valore 2.50
```