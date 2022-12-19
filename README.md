# Galang-Dwiwana-Thabrani-IF-B
# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Galang Dwiwana Thabrani
<br>NIM		:	1227050048
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
PROGAM MENENTUKAN MATRIKS YANG  HABIS DIBAGI 3,5,7
## Source Code

```
#include <iostream>
#include <iomanip>
using namespace std;
int main(){
    
	int array[100][100], jumlahBaris, jumlahKolom, a, b;
  cout<< "NAMA : GALANG DWIWANA THABRANI"<<endl;
  cout<< "NIM  : 1227050048"<<endl;
  cout<< "=========================================================" << endl;
  cout<< "#PROGAM MENENTUKAN MATRIKS YANG  HABIS DIBAGI 3,5,7#" << endl;
  cout<< "=========================================================" << endl;
 
    cout<<"Input jumlah baris: "<<endl;
	cin>>jumlahBaris;
    cout<<"Input jumlah kolom: "<<endl;
	cin>>jumlahKolom;
    cout << endl;

    for(a = 0; a < jumlahBaris; a++){
     for(b = 0; b < jumlahKolom; b++){
            cout << "Baris " <<a+1<<", kolom "<<b+1<< " = ";
            cin >> array[a][b];
        }
        cout << endl;
    }

    cout << "Hasil input: " << endl;

    for(a = 0; a < jumlahBaris; a++){
    for(b = 0; b < jumlahKolom; b++){
        cout << setw(3) << array[a][b] << " ";
    }
    cout << endl;
    }
    cout<<"=================================================="<<endl;
    cout <<"bilangan yang tidak bisa dibagi 3,5,7 : " << endl;

    for(a = 0; a < jumlahBaris ; a++){
     for(b = 0; b < jumlahKolom; b++){
      if(array[a][b] % 3 == 0 || array[a][b] % 5 == 0 || array[a][b] % 7 == 0) {
        cout << setw(3) << array[a][b] << " ";
        }
    }
    cout << endl;
    }
    return 0;
}
```

## Output

```
NAMA : GALANG DWIWANA THABRANI
NIM  : 1227050048
=========================================================
#PROGAM MENENTUKAN MATRIKS YANG  HABIS DIBAGI 3,5,7#
=========================================================
Input jumlah baris:
2
Input jumlah kolom:
2

Baris 1, kolom 1 = 3
Baris 1, kolom 2 = 7

Baris 2, kolom 1 = 8
Baris 2, kolom 2 = 9

Hasil input:
  3   7
  8   9
==================================================
bilangan yang habis bisa dibagi 3,5,7 :
  3   7
  9


```

