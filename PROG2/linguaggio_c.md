---
title:  'Linguaggio C'
---

# Linguaggio C

In C una variabile è una porzione di memoria, in particolare:

- La quantità di memoria allocata
- Dove la variabile è allocata
- Il contenuto della cella di memoria

## Caratteristiche del linguaggio

### Tipizzazione

- Linguaggi staticamente tipizzati, come C, a tempo di compilazione, il compilatore conosce il tipo
- Linguaggi dinamicamente tipizzati, il tipo associato alla variabile è associato durante il runtime

### Type-safe

Un linguaggio è type-safe se le operazioni sono coerenti con i tipi, in caso contrario da un errore a runtime o a compile-time. Ad esempio in un array di 5 elementi, non posso accedere all'indice 7. **C non è type-safe**

### Type-Sound

Un linguaggio si dice Type-Sound se una volta compilato il programma, a runtime non ci saranno problemi con i tipi.

Se un linguaggio non è Type-safe e non è staticamente tipizzato, non può essere Type-Sound.

C ha queste caratteristiche per produrre programmi efficienti al massimo.

## Principio del privilegio minimo

Bisogna eseguire il codice sempre al privilegio minimo.
 
Ad esempio in C, se un valore è costante usiamo la keyword `const`.

Ad esempio:

- Puntatore non costante a dati non costanti oppure puntatore costante a dati non costante.
- Puntatore non costante a dati costanti e viceversa

### Uso di stdbool.h

L'uso di stdbool.h è vietato, usare il tipo `_Bool`

## Processo di compilazione

- Preprocessione, esegue le istruzioni al preprocessore
- Compilazione, produce file assembly
- Assemblamento, dall'assembly produce in file oggetto
- Linking, unisce i file oggetti per produrre un programma

### Tree progetto C

- src/ codice sorgente .c
- include/ file header .h
- bin/ file compilati