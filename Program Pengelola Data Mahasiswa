#include <iostream>
#include <vector>
#include <fstream>
#include <algorithm>

using namespace std;

struct Mahasiswa {
    string NIM;
    string nama;
    float nilaiAkhir;
};

void tambahData(vector<Mahasiswa>& data) {
    int jumlah;
    cout << "Masukkan jumlah mahasiswa: ";
    cin >> jumlah;
    for (int i = 0; i < jumlah; i++) {
        Mahasiswa mhs;
        cout << "Masukkan NIM Mahasiswa ke-" << i+1 << ": ";
        cin >> mhs.NIM;
        cout << "Masukkan Nama Mahasiswa ke-" << i+1 << ": ";
        cin >> mhs.nama;
        cout << "Masukkan Nilai Akhir Mahasiswa ke-" << i+1 << ": ";
        cin >> mhs.nilaiAkhir;
        data.push_back(mhs);
    }
}

void tampilkanData(const vector<Mahasiswa>& data) {
    for (const auto& mhs : data) {
        cout << "NIM: " << mhs.NIM << ", Nama: " << mhs.nama << ", Nilai Akhir: " << mhs.nilaiAkhir << "\n";
    }
}

void cariData(const vector<Mahasiswa>& data) {
    string nimCari;
    cout << "Masukkan NIM yang ingin dicari: ";
    cin >> nimCari;
    for (const auto& mhs : data) {
        if (mhs.NIM == nimCari) {
            cout << "Data ditemukan: NIM: " << mhs.NIM << ", Nama: " << mhs.nama << ", Nilai Akhir: " << mhs.nilaiAkhir << "\n";
            return;
        }
    }
    cout << "Data tidak ditemukan.\n";
}

void urutkanData(vector<Mahasiswa>& data) {
    sort(data.begin(), data.end(), [](Mahasiswa a, Mahasiswa b) {
        return a.nilaiAkhir > b.nilaiAkhir;
    });
    cout << "Data berhasil diurutkan berdasarkan Nilai Akhir (descending).\n";
}

void simpanKeBerkas(const vector<Mahasiswa>& data) {
    ofstream file("data_mahasiswa.txt");
    for (const auto& mhs : data) {
        file << mhs.NIM << "," << mhs.nama << "," << mhs.nilaiAkhir << "\n";
    }
    file.close();
    cout << "Data berhasil disimpan ke berkas.\n";
}

void bacaDariBerkas(vector<Mahasiswa>& data) {
    ifstream file("data_mahasiswa.txt");
    Mahasiswa mhs;
    string line;
    data.clear();
    while (getline(file, line)) {
        size_t pos1 = line.find(',');
        size_t pos2 = line.rfind(',');
        mhs.NIM = line.substr(0, pos1);
        mhs.nama = line.substr(pos1 + 1, pos2 - pos1 - 1);
        mhs.nilaiAkhir = stof(line.substr(pos2 + 1));
        data.push_back(mhs);
    }
    file.close();
    cout << "Data berhasil dibaca dari berkas.\n";
}

int main() {
    vector<Mahasiswa> data;
    int pilihan;
    do {
        cout << "\nMenu Utama:\n";
        cout << "1. Tambah Data Mahasiswa\n";
        cout << "2. Tampilkan Semua Data\n";
        cout << "3. Cari Data Mahasiswa\n";
        cout << "4. Urutkan Data\n";
        cout << "5. Simpan Data ke Berkas\n";
        cout << "6. Baca Data dari Berkas\n";
        cout << "7. Keluar\n";
        cout << "Pilih opsi (1-7): ";
        cin >> pilihan;

        switch (pilihan) {
            case 1: tambahData(data); break;
            case 2: tampilkanData(data); break;
            case 3: cariData(data); break;
            case 4: urutkanData(data); break;
            case 5: simpanKeBerkas(data); break;
            case 6: bacaDariBerkas(data); break;
            case 7: cout << "Keluar dari program.\n"; break;
            default: cout << "Pilihan tidak valid!\n";
        }
    } while (pilihan != 7);

    return 0;
}
