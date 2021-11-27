# TUGAS-ALGORITMA-PERULANGAN

#include<iostream>
  
// itu abis include diatas dikasih iostream ya, sebenernya udh ditulis tapi gak tampil, gak tau lh tulis aja :) #SALAMDARIYGBUAT

using namespace std;

int main() {

	
	// TUGAS TEORI
	
	string namamhs, nama_mtkuliah, indeks_nilai;
	int nim, kode_mtkuliah, nilai_mtkuliah;
	
	cout << "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n";
	cout << "~~ PROGRAM MENENTUKAN INDEKS NILAI MAHASISWA ~~\n";
	cout << "~~ NAMA \t:	M TAUFIK FADILLAH    ~~\n";
	cout << "~~ NIM  \t: 	0702212109           ~~\n";
	cout << "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n";
	
	cout << "Masukan Nama Mahasiswa  --> "; cin >> namamhs;
	cout << "Masukan Nilai Mahasiswa --> "; cin >> nilai_mtkuliah;
	
	if ( nilai_mtkuliah > 80 ) {
		indeks_nilai = "A";
	} else if ( nilai_mtkuliah > 70 && nilai_mtkuliah < 80 ) {
		indeks_nilai = "B";
	} else if ( nilai_mtkuliah > 55 && nilai_mtkuliah < 70 ) {
		indeks_nilai = "C";
	} else if ( nilai_mtkuliah > 40 && nilai_mtkuliah < 50 ) {
		indeks_nilai = "D";
	} else {
		indeks_nilai = "E";
	}
	
	cout << "---------------------------------------------\n";
	
	cout << "Nama Mahasiswa 		--> " << namamhs << "\n";
	cout << "Nilai Ujian    		--> " << nilai_mtkuliah << "\n";
	cout << "Indeks Nilai   		--> " << indeks_nilai << "\n";

	
	
	
	// TUGAS PRAKTEK

	// NO --> 1 
		
	int tahun, kota_a, kota_b;
	double kota_a_grow, kota_b_grow;
	
	cout << "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n";
	cout << "~~    Menghitung Pada Tahun Keberapa Jumlah 	~~\n";
	cout << "~~  Penduduk Kota A Lebih Banyak Dari Kota B   ~~\n";
	cout << "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n";
	cout << "~~ NAMA \t:	M TAUFIK FADILLAH       ~~\n";
	cout << "~~ NIM  \t: 	0702212109              ~~\n";
	cout << "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n";
	
	cout << "Masukan Tahun Awal --> "; cin >> tahun;
	cout << "Masukan Jumlah Penduduk Kota A 			      --> "; cin >> kota_a;
	cout << "Presentase Pertumbuhan Penduduk Kota A Contoh 7%=0.07 --> "; cin >> kota_a_grow;
	
	cout << "\n";
	
	cout << "Masukan Jumlah Penduduk Kota B 			      --> "; cin >> kota_b;
	cout << "Presentase Pertumbuhan Penduduk Kota B Contoh 7%=0.07 --> "; cin >> kota_b_grow;
	
	while ( kota_a <= kota_b ) {
		kota_a += kota_a * kota_a_grow;
		kota_b += kota_b * kota_b_grow;
		tahun++;
	}
	
	cout << "---------------------------------------------------------\n";
	cout << "Penduduk kota A melebihi kota B pada tahun --> " << tahun << "\n";
	cout << "Jumlah penduduk kota A pada tahun " << tahun << ", adalah " << kota_a << "\n";
	cout << "Jumlah penduduk kota B pada tahun " << tahun << ", adalah " << kota_b;
	
	
	
	
	// NO --> 2

	int n, awal, hasil;	
	
	cout << "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n";
	cout << "~~ Menghitung Bilangan Pangkat 3 Yang Diperoleh ~~\n";
	cout << "~~       Dengan Penjumlahan Suku-Sukunya        ~~\n";
	cout << "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n";
	cout << "~~ NAMA \t:	M TAUFIK FADILLAH       ~~\n";
	cout << "~~ NIM  \t: 	0702212109              ~~\n";
	cout << "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n";
		
	cout << "Masukan angka --> "; cin >> n;
	cout << n << "*3 = ";
	
	awal = n * ( n - 1 ) + 1;
	cout << awal;
	
	hasil = awal;
	for ( int i = 2; i <= n; i++ ) {
		awal = awal + 2;
		cout << " + " << awal;
	
		hasil += awal; 
	}
	
	cout << " = " << hasil;
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
		
}
	


