#praktikum3
Latihan1.cpp : Program Menghitung bilangan terbesar sebanyak jumlah "n"

Alur algoritma

    Mendeklarasikan variabel int a,max,n sebagai variabel input
    Membaca input dari keyboard cin >> n
    Membandingkan nilai variabel A dengan variabel max jika a>max
    Bandingkan kembali kedua variabel sebanyak jumlah n atau bilangan yang di input sampai menemukan hasil a=max maka cetaklah.
    Print bilangan terbesar dari semua bilangan yang di inputkan.

Flowchart Program flowchart

code program lengkap :

#include<iostream>

using namespace std;

int main() {
    int i=0;
    int max=0;
    int n,a;

    cout << "Masukkan jumlah bilangan: ";
    cin >> n;

    for (i;i<n;i++) {
        cout << "Masukkan bilangan ke-" << i+1 << ": ";
        cin >> a;

        if (a > max)
            max = a;
    }

    cout << "Bilangan terbesar adalah: " << max << endl;
}

hasilnya :

hasilnya
Latihan2.cpp : Program mengurutkan bilangan terkecil hingga ke terbesar

Alur algoritma

    Mendeklarasikan variabel int A,B,C sebagai variabel input s2. Membaca input dari keyboard cin >> A >> B >> C
    Membandingkan nilai variabel A dengan variabel B jika A lebih kecil daripada B
    Bandingkan kembali variabel B dengan variabel C
    Jika kondisi TRUE , Maka cetaklah bilangan secara berurutan dari yanng terkecil-terbesar yaitu A,B,C
    Jika kondisi FALSE , bandingkan kembali variabel A dengan variabel C jika A lebih kecil dari C
    Jika kondisi TRUE , Maka cetaklah bilangan secara berurutan dari yang terkecil-terbesar yaitu A,C,B
    Jika kondisi FALSE , Maka cetaklah bilangan secara berurutan dari yang terkecil-terbesar yaitu C,A,B
    Kemudian jika A lebih kecil dari C
    Jika kondisi TRUE , Maka cetaklah bilangan secara berurutan dari yang terkecil-terbesar yaitu B,A,C
    Jika kondisi FALSE , Bandingkan kembali variabel B dengan variabel C jika B lebih kecil dari C
    Jika kondisi TRUE , Maka cetaklah bilangan secara berurutan dari yang terkecil-terbesar yaitu B,C,A
    Jika kondisi FALSE , Maka cetaklah bilangan secara berurutan dari yang terkecil-terbesar yaitu C,B,A
    Lalu, END.

Flowchart Program flowchart

code program lengkap :

#include<iostream>

using namespace std;

int main(){
    int A,B,C;

    cout << "Masukkan bilangan A: "; cin >> A;
    cout << "Masukkan bilangan B: "; cin >> B;
    cout << "Masukkan bilangan C: "; cin >> C;

    if (A<B) {
        if (B<C)
            cout << "Urutan bilangan: " << A << ", " << B << ", " << C << endl;
        else {
            if (A<C)
                cout << "Urutan bilangan: " << A << ", " << C << ", " << B << endl;
            else
                cout << "Urutan bilangan: " << C << ", " << A << ", " << B << endl;
        }
    } else {
        if (A<C)
            cout << "Urutan bilangan: " << B << ", " << A << ", " << C << endl;
        else {
            if (B<C)
                cout << "Urutan bilangan: "<< B << ", " << C << ", " << A << endl;
            else
                cout << "Urutan bilangan: "<< C << ", " << B << ", " << A << endl;
        }
    }
}

hasilnya :

hasilnya
Latihan3.cpp : Program mencetak nilai tengah dari 3 buah bilangan yang diinputkan

Alur algoritma

    Mendeklarasikan variabel int A,B,C sebagai variabel input
    Membaca input dari keyboard cin << A << B << C
    Membandingkan nilai variabel A dengan variabel B jika A lebih kecil daripada B
    Bandingkan kembali variabel B dengan variabel C
    Jika kondisi TRUE , Maka cetaklah bilangan tengah dari A,B,C yaitu B
    Jika kondisi FALSE , bandingkan kembali variabel A dengan variabel C jika A lebih kecil dari C
    Jika kondisi TRUE , Maka cetaklah bilangan tengah dari A,C,B yaitu C
    Jika kondisi FALSE , Maka cetaklah bilangan tengah dari C,A,B yaitu A
    Kemudian jika A lebih kecil dari C
    Jika kondisi TRUE , Maka cetaklah bilangan tengah dari B,A,C yaitu A
    Jika kondisi FALSE , Bandingkan kembali variabel B dengan variabel C jika B lebih kecil dari C
    Jika kondisi TRUE , Maka cetaklah bilangan tengah dari B,C,A yaitu C
    Jika kondisi FALSE , Maka cetaklah bilangan tengah dari C,B,A yaitu B
    Lalu, END.

Flowchart Program flowchart

code program lengkap :

#include<iostream>

using namespace std;

int main () {

    int A,B,C;
    cout<<"Masukan bilangan 1: ";
    cin>> A;
    cout<<"Masukan bilangan 2: ";
    cin>> B;
    cout<<"Masukan bilangan 3: ";
    cin>> C;

    if (A<B) {
        if (B<C)
            cout<< "Bilangan tengah adalah:" << B << endl;
    else
        if (A<C)
            cout<< "Bilangan tengah adalah:" << C << endl;
        else  cout<< "Bilangan tengah adalah:" << A << endl;
    }else{
    if (A<C)
        cout << "Bilangan tengah adalah: " << A << endl;
    else
        if (B<C)

        cout << "Bilangan tengah adalah: " << C << endl;
    else
         cout << "Bilangan tengah adalah: " << B << endl;
    }
}

hasilnya :

hasilnya

**TERIMA KASIH**

praktikum3
