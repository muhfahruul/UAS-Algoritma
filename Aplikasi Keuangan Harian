#include <iostream>
#include <string>

using namespace std;

int main() {
    double saldoAwal, totalPengeluaran = 0;
    int pilihan;

    cout << "Selamat datang di Aplikasi Keuangan Harian!\n";
    cout << "Masukkan saldo awal Anda: ";
    cin >> saldoAwal;

    do {
        cout << "\nMenu Utama:\n";
        cout << "1. Tambah Pengeluaran\n";
        cout << "2. Tampilkan Total Pengeluaran\n";
        cout << "3. Tampilkan Sisa Saldo\n";
        cout << "4. Keluar\n";
        cout << "Pilih opsi (1-4): ";
        cin >> pilihan;

        if (pilihan == 1) {
            string kategori;
            double jumlah;
            cout << "Masukkan nama kategori pengeluaran: ";
            cin >> kategori;
            cout << "Masukkan jumlah pengeluaran: ";
            cin >> jumlah;
            if (jumlah > saldoAwal) {
                cout << "Pengeluaran melebihi saldo Anda!\n";
            } else {
                totalPengeluaran += jumlah;
                saldoAwal -= jumlah;
                cout << "Pengeluaran berhasil ditambahkan!\n";
            }
        } else if (pilihan == 2) {
            cout << "Total pengeluaran Anda: " << totalPengeluaran << "\n";
        } else if (pilihan == 3) {
            cout << "Sisa saldo Anda: " << saldoAwal << "\n";
        } else if (pilihan != 4) {
            cout << "Pilihan tidak valid!\n";
        }
    } while (pilihan != 4);

    cout << "Terima kasih telah menggunakan Aplikasi Keuangan Harian!\n";
    return 0;
}
