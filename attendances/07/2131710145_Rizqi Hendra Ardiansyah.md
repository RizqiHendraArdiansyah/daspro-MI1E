## NAMA : RIZQI HENDRA ARDIANSYAH
## NIM     : 2131710145

## JOBSHEET 7

## PERULANGAN 1

### Tujuan

Mahasiswa mampu menyelesaikan permasalahan/studi kasus menggunakan sintaks perulangan 1 dan mengimplemantasikannya dalam bahasa pemrogaman java.

### Alat dan Bahan
+ PC/laptop
+ Browser(chrome, firefox, safari)
+ Koneksi internet

### Praktikum

#### Percobaan 1 : Penggunaan for, while dan do-while

#### Waktu percobaan : 40 menit

1. Perhatikan flowchart perulangan for dibawah ini!

    <p align="left">
    <img width="197" height="259" src="images/flowchartFaktorial.png">
    </p>
    

> Flowchart diatas digunakan untuk menghitung nilai faktorial, selanjutnya kita akan membuat programnya berdasarkan
> flowchart di atas!

2. Tambahkan library Scanner, deklarasi Scanner, dan buat variabel angka untuk menampung data yang diinput melalui keyboard




```Java
import java.util.Scanner;
Scanner input = new Scanner(System.in);
```

3. Buatlah deklarasi dan inisialisasi variabel faktorial sesuai dengan flowchart diatas


```Java
int angka;
int faktorial = 1;
```

4. Tambahkan struktur perulangan untuk menghitung hasil faktorial sebuah nilai yang diinputkan menggunakan for
    
    <p align="left">
    <img width="696" height="124" src="images/for.jpg" align="left">
    </p>


```Java
System.out.println("=====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN FOR=====");
System.out.print("Masukkan Bilangan : ");
angka = input.nextInt();
for(int i=1; i<=angka; i++)
    faktorial*=i;
System.out.print("Nilai faktorial bilangan tersebut adalah : "+ faktorial);

```

    =====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN FOR=====
    Masukkan Bilangan : 4
    Nilai faktorial bilangan tersebut adalah : 24

5. Ubah nilai variabel faktorial seperti semula. Kemudian gunakan struktur perulangan while untuk menghitung hasil faktorial sebuah nilai yang diinputkan
    
    <p align="left">
    <img width="696" height="124" src="images/while.jpg" align="left">
    </p>


```Java
faktorial=1;
System.out.println("=====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN WHILE=====");
System.out.print("Masukkan Bilangan : ");
angka = input.nextInt();
int i=1;
while(i<=angka){
    faktorial*=i;
    i++;
}
System.out.print("Nilai faktorial bilangan tersebut adalah : "+ faktorial);
```

    =====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN WHILE=====
    Masukkan Bilangan : 5
    Nilai faktorial bilangan tersebut adalah : 120

6. Kembalikan lagi nilai variabel faktorial seperti semula. Gunakan struktur perulangan do-while untuk menghitung hasil faktorial sebuah nilai yang diinputkan
    
    <p align="left">
    <img width="696" height="124" src="images/dowhile.jpg" align="left">
    </p>

// Ketik kode program di atas di bawah sini



```Java
faktorial=1;
System.out.println("=====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN DO-WHILE=====");
System.out.print("Masukkan Bilangan : ");
angka = input.nextInt();
int i=1;
do{
   faktorial*=i;
   i++;
}
while(i<=angka);
System.out.print("Nilai faktorial bilangan tersebut adalah : "+ faktorial);
```

    =====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN DO-WHILE=====
    Masukkan Bilangan : 6
    Nilai faktorial bilangan tersebut adalah : 720

##### Pertanyaan
1. Pada program diatas, apakah kegunaan baris berikut?
<p align="left">
    <img src="images/hitungFaktorial.jpg" align="left">
    </p>

#### Jawab 
1.Kegunaan dari faktorial*=i adalah untuk mengkalikan nilai dari variabel faktorial dengan variabel i


2. Modifikasi program diatas dibagian struktur pemilihannya sehingga hasilnya menjadi seperti di bawah ini:
<p align="left">
    <img src="images/modifP1.jpg" align="left">
    </p>


```Java
faktorial = 1;
System.out.println("=====PROGRAM MENGHITUNG NILAI FAKTORIAL=====");
System.out.print("Masukan Bilangan : ");
angka = input.nextInt();
int i = 1 ;
System.out.print(angka + "Faktorial = ");
for(i = 1;i <= angka  ; i++){
    faktorial *= i;
//     System.out.print(angka + "Faktorial = 1x" );
    if(i == angka){
        System.out.print(i);
    }else{
        System.out.print(i + "x");
    }
}
System.out.println(" = " + faktorial);
```

    =====PROGRAM MENGHITUNG NILAI FAKTORIAL=====
    Masukan Bilangan : 5
    5Faktorial = 1x2x3x4x5 = 120
    

#### Percobaan 2 : Keluar dari perulangan menggunakan break

#### Waktu percobaan : 40 menit

1. Buatlah perulangan dengan menggunakan for yang memanfaatkan keyword break
<p align="left">
    <img width="696" height="124" src="images/for2.jpg" align="left">
    </p>


```Java
Scanner input=new Scanner(System.in);
int angka,total;
System.out.println("===PROGRAM FOR LOOP DENGAN BREAK===");
for(total=0;true;){
    System.out.print("Masukkan Bilangan : ");
    angka=input.nextInt();
    total+=angka;
    if(total>50) break;
}
System.out.println("Jumlah angka-angka yang telah dimasukkan : "+total);
```

    ===PROGRAM FOR LOOP DENGAN BREAK===
    Masukkan Bilangan : 10
    Masukkan Bilangan : 20
    Masukkan Bilangan : 30
    Jumlah angka-angka yang telah dimasukkan : 60
    

2. Buat perulangan yang sama dengan struktur perulangan while
<p align="left">
    <img width="696" height="124" src="images/while2.jpg" align="left">
    </p>


```Java
int angka,total;
System.out.println("===PROGRAM WHILE LOOP DENGAN BREAK===");
total=0;
while(true){
    System.out.print("Masukkan Bilangan : ");
    angka=input.nextInt();
    total+=angka;
    if(total>50) break;
}
System.out.println("Jumlah angka-angka yang telah dimasukkan : "+total);

```

    ===PROGRAM WHILE LOOP DENGAN BREAK===
    Masukkan Bilangan : 40
    Masukkan Bilangan : 30
    Jumlah angka-angka yang telah dimasukkan : 70
    

3. Tuliskan perulangan diatas dalam struktur do-while
    <p align="left">
    <img width="696" height="124" src="images/dowhile2.jpg" align="left">
    </p>


```Java
int angka,total;
System.out.println("===PROGRAM DO-WHILE LOOP DENGAN BREAK===");
total=0;
do
{
    System.out.print("Masukkan Bilangan : ");
    angka=input.nextInt();
    total+=angka;
    if(total>50) break;
}
while(true);
System.out.println("Jumlah angka-angka yang telah dimasukkan : "+total);

```

    ===PROGRAM DO-WHILE LOOP DENGAN BREAK===
    Masukkan Bilangan : 30
    Masukkan Bilangan : 25
    Jumlah angka-angka yang telah dimasukkan : 55
    

##### Pertanyaan
1. Jelaskan fungsi kode program yang telah dibuat pada percobaan diatas!

#### Jawab 
Program diatas digunakan untuk memasukkan bilangan sampe 50, ketika terdapat bilangan yang lebih dari angka 50, maka program tersebut akan menjumlahkan bilangan-bilangan yang telah dimasukkan sampai bilangan terakhir yang lebih dari 50

2. Jelaskan fungsi kode berikut!
    <p align="left">
    <img src="images/forPertanyaan2.jpg" align="left">
    </p>


#### Jawab
Fungsi kode tersebut adalah nilai dari variabel total dimulai dari nol,lalu misal hasilnya true maka program tersebut dapat berjalan dengan lancar


#### Percobaan 3 : Keluar dari step perulangan menggunakan continue

#### Waktu percobaan : 40 menit

1. Buat program looping menggunakan struktur perulangan for seperti di bawah ini: 
<p align="left">
    <img src="images/forContinue.jpg" align="left">
    </p>



```Java
Scanner input=new Scanner(System.in);
int angka, total, count;
double avg;
count=0;
System.out.println("===PROGRAM FOR LOOP DENGAN CONTINUE===");
for(int i=0;i<5;i++){
    System.out.print("Masukkan Bilangan : ");
    angka=input.nextInt();
    if(angka>=50) continue;
    total+=angka;
    count++;
}
System.out.println("Jumlah angka-angka yang kurang dari 50: "+total);
avg=(double)total/count;
System.out.println("Rata-rata angka yang kurang dari 50: "+avg);


```

    ===PROGRAM FOR LOOP DENGAN CONTINUE===
    Masukkan Bilangan : 10
    Masukkan Bilangan : 20
    Masukkan Bilangan : 30
    Masukkan Bilangan : 40
    Masukkan Bilangan : 50
    Jumlah angka-angka yang kurang dari 50: 100
    Rata-rata angka yang kurang dari 50: 25.0
    

5. Jalankan program. Amati apa yang terjadi!

##### Pertanyaan
1. Jelaskan Perbedaan dari percobaan 2 dan percobaan 3

#### Jawab
Perbedaannya adalah pada percobaan ke 2 menggunakan "break" yang digunakan untuk menghentikan paksa proses perulangan yang berlangsung, Sedangkan pada percobaan 3 menggunakan "continue" yang digunakan untuk menghentikan perulangan yang saat terjadi (1 perulangan saja), kemudian melanjutkan perulangan berikutnya atau bisa disebut juga untuk melewati 1 perulangan tambahan.


2. Jelaskan apa fungsi perintah kode program dibawah ini?
<p align="left">
    <img width="352" height="79" src="images/continuePertanyaan.jpg" align="left">
    </p>

#### Jawab

- Fungsi program if(angka>=50) continue; yaitu ketika kita memasukkan angka lebih besar sama dengan 50 maka program akan melewati perulangan,namun program tersebut akan langsung lanjut ke tahapan berikutnya. 

- Fungsi program total+=angka; yaitu ketika kita memasukkan angka yang dimasukkan sesuai dengan syarat, maka akan terjadi perulangan/looping. 

- Fungsi program count++; yaitu untuk mencatat/menghitung looping pada program yang telah ditentukan.


### Tugas

#### Waktu pengerjaan Tugas: 140 menit

1. Buatlah program yang meminta masukan user sebuah bilangan bulat N (N > 0). Program kemudian menampilkan penjumlahan N bilangan genap positif pertama (bilangan genap ≥ 0).
Contoh: 
    •	Jika user memasukkan N = 10, program akan menghitung banyaknya jumlah bilangan positive di dalam range bilangan 1-10   kemudian menampilkan penjumlahan bilangan positive bilangan bilangan diantara 1-10 yaitu : 
        0 + 2 + 4 + 6 + 10 = 30. 
        Setelah itu program akan menampilkan rata-rata dari bilangan positive yang telah dijumlahkan tadi.
    •	Contoh output program dan flowchart
<br/><img width="303" height="529" src="images/hasilTugasFc.jpg" align="left"><br/>
  

<br/><img width="303" height="529" src="images/fcTugasJS7.png" align="left">



```Java
import java.util.Scanner;
Scanner input = new Scanner(System.in);
int bil, jbilgenap;
int totalgenap = 0;
double avg;

System.out.print("Masukkan Bilangan\t\t\t\t\t\t\t: ");
bil = input.nextInt();
jbilgenap = bil/2;
System.out.println("Banyak bilangan genap dari 1 sampai " + bil + " Adalah\t\t\t\t: " + jbilgenap);
System.out.print("Angka Genap dalam range tersebut adalah\t\t\t\t\t: ");
for(int i = 1; i <= bil; i++){
    if(i%2!=0){
        continue;
    }else{
        if(i == bil){
            System.out.println(i);
        }else{
            if (bil % 2 == 0){
                System.out.print(i + ", ");
            }else{
                System.out.println(i);
            }
        }
        totalgenap += i;
    }
}
    avg = totalgenap / jbilgenap;
    System.out.println("Hasil Penjumlahan Bilangan Genap dari 1 sampai " + bil + " adalah\t\t: " + totalgenap);
    System.out.println("Rata Rata Bilangan Genap dari 1 sampai " + bil + " adalah\t\t\t: " + avg);

```

    Masukkan Bilangan							: 10
    Banyak bilangan genap dari 1 sampai 10 Adalah				: 5
    Angka Genap dalam range tersebut adalah					: 2, 4, 6, 8, 10
    Hasil Penjumlahan Bilangan Genap dari 1 sampai 10 adalah		: 30
    Rata Rata Bilangan Genap dari 1 sampai 10 adalah			: 6.0
    

2. Buatlah program untuk menampilkan angka 1 hingga angka masukan pengguna secara berurutan dan melompati angka kelipatan 5. Seperti tampilan di bawah ini
<p align="left">
<img width="184" height="328" src="images/tugas1.jpg" align="left">
</p>


```Java
import java.util.Scanner;
Scanner s=new Scanner(System.in);
int x, i;
System.out.print("Masukkan Bilangan : ");
    i = s.nextInt();

for(x=1; x<=i; x++) {
if (x%5==0) continue;
System.out.println(x);
}
```

    Masukkan Bilangan : 18
    1
    2
    3
    4
    6
    7
    8
    9
    11
    12
    13
    14
    16
    17
    18
    

## 3. Buatlah sebuah program yang menampilkan deret bilangan fibonacci sebagai berikut. Dimana bilangan yang terletak di sebelah kanan adalah hasil penjumlahan dari 2 bilangan sebelumnya
 <p align="left">
    <img width="451" height="226" src="images/fibo.png" align="left">
    </p>



```Java
import java.util.Scanner;
        int a, b, c, d;
        Scanner input = new Scanner(System.in);
        System.out.print("Masukan banyak bilangan yang ingin ditampilkan: ");
        a = input.nextInt();
        b = 0;
        c = 1;
        d = 1;
        for (int i =1; i <= a; i++){
            d = b + c;
            System.out.printf("sum of: %d + %d = %d\n",b,c,d);
            b = c;
            c = d;
        }
```

    Masukan banyak bilangan yang ingin ditampilkan: 10
    sum of: 0 + 1 = 1
    sum of: 1 + 1 = 2
    sum of: 1 + 2 = 3
    sum of: 2 + 3 = 5
    sum of: 3 + 5 = 8
    sum of: 5 + 8 = 13
    sum of: 8 + 13 = 21
    sum of: 13 + 21 = 34
    sum of: 21 + 34 = 55
    sum of: 34 + 55 = 89
    


```Java

```
