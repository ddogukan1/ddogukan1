Veri yapıları ve Algoritmalar
[22,27,16,2,18,6] -> Ekleme Sıralaması

aşama : 2 en küçük sayı olduğu için en başa geçer. [2,27,16,22,18,6]
aşama : 6, diğer en küçük sayı olduğu için 2'nin yanında geçer. [2,6,16,22,18,27]
aşama : 18, 22den küçük olduğu için 16'nın yanına geçer. [2,6,16,18,22,27]
: Diğer üçlüden küçükten büyüğe göre sıralandığı için işlem bitmiştir.
Dizideki eleman sayısı n olsun. Big-O yöntemine göre sıralama yapılırken işlem sayısı da n olur. Son işlem sayısı 1 olana kadar devam eder. [22,27,16,2,18,6] dizisinde 6 tane eleman vardır, yani 6 tane işlem yapılması gerekir. zengin ki,

n-> 6 tane işlem,
en küçük eleman (yani birinci) bulmak için (n-1)-> 6-1=5 tane işlem,
ikinci elemanı bulmak için (n-2)-> 6-2=4 tane işlem,
Üçüncü öğeyi işlemi bulmak için (n-3)-> 6-3=3 tane,
dördüncü elemanı bulmak için (n-4)-> 6-4=2 tane işlem yapılır.
Altı elemanlı dizi olduğu için daha fazla işlem yapılmasına gerek yoktur çünkü son eleman bir sonraki elemandır.-
Bu listede n+(n-1)+(n-2)+(n-3)+(n-4)+1 kadar işlem yapılır. Bu işlemin formülü: [n(n+1)]/2'dir. Bu formüller sadeleştirilerek: (n²+n)/2 elde edilir.
Big-O Notation'da kat sayısı önemsizdir; yani domine eden fonksiyon n² alınır.
Büyük-O değeri = O(n²)
Zaman araştırmaları: Dizi sıralandıktan sonra 18 sayı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

[2,6,16,18,22,27] olarak sonuçlandığı için ve "18" ortada kaldığı için Ortalama vaka'e girer.

[7,3,5,8,2,9,4,15,6] dizisinin Seçimi Sıralama'ya göre ilk 4 adımını attı.

En küçük "2" olduğu için, 2 ve 7'nin yerini değiştireceğiz. [2,3,5,8,7,9,4,15,6] n + (n-1)
3 diğer en küçük olduğu için olduğu yerde kalır, 4 rakam 3 ve 5 üzerine yerleştirilir. [2,3,4,5,8,7,9,15,6] ( n-2)
6 , 5 ve 8 tane geçer. [2,3,4,5,6,8,7,9,15] (n-3)
7, 6 ve 8 aşaması geçer. [2,3,4,5,6,7,8,9,15] (n-4)
