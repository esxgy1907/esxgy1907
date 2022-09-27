#include <iostream>
#include <conio.h>
using namespace std;
struct buku

{ 
int kodeB,sewa,stock;
char judul;
int b;
}buku[200];
struct pinjam
{
int kodepinjam,tanggalpinjam,tanggalkembali,dipinjam;
char nama[50];
char alamat [50];
char status;
}pinjambuku[200];

int main () {
system("cls");

int jumlahbuku,jumlahpinjam,kodepinjam,stock;
char yn,ch,temp;

login:
string user ="";
string pass ="";
cout<<"\n\n\n\n\n\n\n\n";
cout<<"\t\t\t --- Peminjaman dan Pengembalian Buku Perpustakaan --- \n\n";
cout<<"\t\t\t username : "; 
cin>>user;
cout<<"\t\t\t password : ";
ch =_getch();
while (ch != 13){
pass.push_back(ch);
cout << '*';
ch = _getch();
}
cout<<endl;
if(user == "upnjatim" && pass == "upn"){
	cout << "\n\n anda berhasil login. \n" <<endl;
	system ("pause");
	system ("cls");
	goto mulaimenu;
}else if (user == "veteran" && pass == "upn"){
	cout << "\n\n anda berhasil login. \n" << endl;
	system ("pause");
	system ("cls");
	goto mulaimenu;
}else{
	cout << "password anda salah \n";
	system ("pause");
	system ("cls");
	goto login;
}
