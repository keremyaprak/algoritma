# Proje 3 #
1. [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.


### CEVAP 1 ###

Bir düğüm her iki tarafa da referans verebiliyor. Sağ ve sol olarak. Sağ tarafından kendinden büyük elemanlar, sol tarafında ise kendinden küçük elemanlar bulunacak.
>root = 7

## AŞAMALAR ##
```
7'ye root olarak belirlemiştik. 7'den sonra gelen 5 değeri 7'den küçük olduğu için 7'nin soluna yazılır.

                7
            5
```

```
1, 7'den ve 5'ten küçük olduğu için hem 7'nin hem de 5'in soluna yazılır.

                7
            5
        1
```

```
8, 7'den büyük olduğu için 7'nin sağına yazılır.

                7
            5       8
        1
```

```
3, 7'den ve 5'ten küçük olduğu için sola ama 1'den büyük olduğu için 1'in sağına ekliyoruz.

                7
            5       8
        1
            3
```

```
6, 7'den küçük olduğu için 7'nin soluna ancak 5'ten büyük olduğu için 5'in sağına yazılır.

                7
            5       8
        1     6
            3
```

```
0, 7'den küçük olduğu için sola, 5 ve 1'den de küçük olduğu için 1'in soluna yazılır.

                7
            5       8
        1     6
     0     3
```

```
9, 7'den büyük olduğu için sağa, aynı zamanda 8'den de büyük onun da sağına yazılır.

                7
            5       8
        1     6        9
     0     3
```

```
4, 7'den küçük olduğu için sola aynı zamanda 5'ten de küçük, 1 ve 3'ten büyük olduğu için 3'ün sağına yazılır.

                7
            5       8
        1     6        9
     0     3
              4
```

```
2, 7'den küçük olduğu için sola aynı zamanda 5'ten de küçük, 1'den büyük o yüzden sağına ama 3'ten küçük olduğu için 3'ün soluna yazılır.

                7
            5       8
        1     6        9
     0     3
         2    4
```