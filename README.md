#include<iostream>
using namespace std;
void DaftarKelasKereta() 
{
    cout << "DAFTAR KELAS KERETA HOGWARTS EXPRESS 5972:" << endl;
    cout << "1. Gryffindor (H)       Rp. 200,000.00" << endl;
    cout << "2. Gryffindor (R)       Rp. 220,000.00" << endl;
    cout << "3. Hufflepuff (CD)      Rp. 250,000.00" << endl;
    cout << "4. Hufflepuff (N)       Rp. 290,000.00" << endl;
    cout << "5. Ravenclaw (L)        Rp. 310,000.00" << endl;
    cout << "6. Ravenclaw (CH)       Rp. 350,000.00" << endl;
    cout << "7. Slytherin (D)        Rp. 490,000.00" << endl;
    cout << "8. Slytherin (BS)       Rp. 580,000.00" << endl;
}

int PilihKelas() 
{
    int pilihan;
    cout << "PILIH JENIS KELAS KERETA (1 - 8) "<<endl;
    cout << "Kelas Nomor : ";
    cin >> pilihan;
    return pilihan;
}

int InputJumlahTiket() 
{
    int jumlah;
    cout << "Jumlah Tiket yang dibeli: ";
    cin >> jumlah;
    return jumlah;
}

int main () 
{
    DaftarKelasKereta();
    
    int NomorKelas = PilihKelas();
    int JumlahTiket = InputJumlahTiket();
    
    int harga[] = {200000, 220000, 250000, 290000, 310000, 350000, 490000, 580000};
    
    int TotalBayar = harga[NomorKelas - 1] * JumlahTiket;
    
    cout << "Total Pembayaran: Rp. " << TotalBayar << endl;

    return 0;
}
