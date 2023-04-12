# Proje 2

## [16,21,11,8,12,22] -> Merge Sort

## 1 - Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.


1 - [16, 21, 11] ve [8, 12, 22] - Dizi ikiye bölünür: 

2 - [16], [21, 11] - Sol taraftaki dizi tekrar ikiye bölünür 

3 - [8], [12, 22] -  Sağ taraftaki dizi tekrar ikiye bölünür

4 - [16] ile [21, 11] birleştirilir ve [11, 16, 21] oluşur.

5 -[12] ile [8] birleştirilir ve [8, 12] oluşur.

6 - [8, 12] ile [11, 16, 21] birleştirilir ve [8, 11, 12, 16, 21] oluşur.

7 - [22] tek başına kaldığı için, son sıralanmış diziye eklenir.

8 - Sıralanmış dizi şudur: [8, 11, 12, 16, 21, 22].


## 2 - Big-O gösterimini yazınız.

1. aşamada n
2. aşamada n/2
3. aşamada n/4    
4. aşamada ...

Ayrıma ve bölme işlemlerinde log(2n) kere toplamda da n-1 kere işlem yapılıyor. Bunları çarptığımızda Sonuç olarak:

Merge Sort'ın zaman karmaşıklığı O(nlogn) 