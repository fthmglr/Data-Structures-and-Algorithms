# Proje 1

### [22,27,16,2,18,6] -> Insertion Sort

### 1 - Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Verilen dizi [22, 27, 16, 2, 18, 6] Insertion Sort algoritması ile sıralandığında aşamalar şu şekilde olur:

[22, 27, 16, 2, 18, 6] - Dizi ilk hali

[22, 27, 16, 2, 18, 6] - İlk eleman (22) zaten sıralı durumda

[16, 22, 27, 2, 18, 6] - İkinci eleman (27) ilk elemandan büyük olduğu için yer değiştirildi

[2, 16, 22, 27, 18, 6] - Üçüncü eleman (16) tek tek baştan karşılaştırılarak sıralandı

[2, 16, 18, 22, 27, 6] - Dördüncü eleman (2) ilk elemandan küçük olduğu için başa yerleştirildi

[2, 6, 16, 18, 22, 27] - Son elemanlar (18 ve 6) sıralandı ve dizi sıralı hale geldi


### 2 - Big-O gösterimini yazınız.

n + (n-1) + (n-2) + (n-3) + (n-4) + (n-5)  = [n(n+1)]/2 = (n^2+n)/2

Ortalama durumda O(n^2) zaman karmaşıklığına sahip olur. Bu, her bir elemanın diğer tüm elemanlarla karşılaştırılması gerektiği için n^2 sayıda karşılaştırma yapılması gerektiği anlamına gelir.


### 3 - Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız 

* Average case: Aradığımız sayının ortada olması
* Worst case: Aradığımız sayının sonda olması
* c: Aradığımsız sayının dizinin en başında olması.

Diziyi sıraladıktan sonra, 18 sayısı 4. pozisyonda yani 3. indexte olacaktır. Bu nedenle, 18 sayısı, doğru pozisyonuna ulaşmak için n-1 karşılaştırma yapmak gerektiğinden, ortalama zamandan daha fazla karşılaştırma yapılacaktır. Burada n, girdi dizisinin uzunluğudur. Bu durumda, n = 6 olduğundan, 5 karşılaştırma yapılacaktır.

Bu nedenle, "Dizi sıralandıktan sonra 18 sayısı "Worst Case" olacaktır.

### 4 - [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

1.adım - [2, 3, 5, 8, 7, 9, 4, 15, 6] - Dizide bulunan en küçük eleman olan 2, 1. pozisyondaki elemanla yer değiştirilir.

2.adım - [2, 3, 4, 8, 7, 9, 5, 15, 6] - Dizide bulunan en küçük eleman 3. pozisyondaki 5'tir. 3. ve 5. pozisyondaki elemanlar yer değiştirilir.

3.adım - [2, 3, 4, 5, 7, 9, 8, 15, 6] - Dizide bulunan en küçük eleman 5. pozisyondaki 7'dir. 5. ve 6. pozisyondaki elemanlar yer değiştirilir.

4.adım - [2, 3, 4, 5, 7, 8, 9, 15, 6] - Dizide bulunan en küçük eleman 7. pozisyondaki 8'dir. 7. ve 8. pozisyondaki elemanlar yer değiştirilir.