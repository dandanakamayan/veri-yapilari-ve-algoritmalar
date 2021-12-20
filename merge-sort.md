# Merge Sort

[16,21,11,8,12,22] -> Merge Sort

1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.

## Cevaplar

    1.
        * [16, 21, 11] -- [8, 12, 22] => ayırma
        * [16, 21] -- [11] --- [8, 12] -- [22] => ayırma 
        * [16] -- [21] --- [11] ---- [8] -- [12] --- [22] => ayırma
        * [16, 21] --- [11] ---- [8, 12] --- [22] => merge
        * [11, 16, 21] ---- [8, 12, 22] => merge
        * [8, 11, 12, 16, 21, 22] => merge


    2.
        n adet işlem -> O(n)

        her adımda n adet işlem yarısı kadar işlem adedine dönüşür:
        2^x = n
        x = logn
        O(logn)

        O(n), O(logn) -> O(nlogn)

       