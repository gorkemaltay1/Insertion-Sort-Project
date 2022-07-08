# Data Structures and Algorithms

## Insertion Sort 

#### Patika Dev Profile : https://app.patika.dev/gorkemaltay

## Proje - 1

[22,27,16,2,18,6] -> Insertion Sort

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
Big-O gösterimini yazınız.
Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.


[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

----
## Çözüm 

### 1- Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
Öncelikle Insertion Sort'un yaptığı iş, bir dizideki en küçük elemanı kontrol edip başa alması işlemidir. Dizinin ilk hali [22,27,16,2,18,6] olduğundan adımlar sırasıyla;

``` [2,22,27,16,18,6] -> [2,6,22,27,16,18] -> [2,6,16,22,27,18] -> [2,6,16,18,22,27] olur. ```
Her elemana tek tek bakıldığından O(n) zamanda işlem yapıldığını gösteriyor.

### 2-Big-O gösterimini yazınız.

Big-O gösterimi için Worst Case'deki time complexity'e bakmamız gerekiyor. Başta n sayıda işlem yapıldığını varsayarsak, bir sonraki adımda n-1 sayıda işlem yapacağız. Bu sekansta devam eden işlemler grubu için yapacağımız toplam işlem sayısı n + n-1 + n-2 ... + 1 olacağından toplam işlem sayımız (n^2+n)/2 olduğundan Big-O notasyonunda bunu O(n^2) olarak gösterebiliriz.

### 3- Time complexity.

O(n^2) olur.

### 4- Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.

Dizi sıralandıktan sonra 18 sayısı Average Case kapsamına girer.

### 5- [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

[2,7,3,5,8,9,4,15,6] -> [2,3,7,5,8,9,4,15,6] -> [2,3,4,7,5,8,9,15,6] -> [2,3,4,5,7,8,9,15,6]
