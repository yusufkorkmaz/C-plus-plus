#include <iostream>
#include <windows.h>
using namespace std;
void coordinateCalculation(int x, int y){
	COORD coordination;
	coordination.X = x;
	coordination.Y = y;
	SetConsoleCursorPosition(GetStdHandle(STD_OUTPUT_HANDLE),coordination);
}
	
int main(int argc, char** argv) {
	int genislik = 50;
	int yukseklik = 10; 
	char a = '-';
	char b = '|';
	for(int i = 0; i<genislik;  i++){cout<<a; Sleep(25);} 
	for(int i = 0; i<yukseklik; i++){coordinateCalculation(genislik-1,i+1); cout<<b<<endl; Sleep(25);}
	for(int i = 1; i<=genislik; i++){coordinateCalculation(genislik-i,yukseklik); cout<<a<<endl; Sleep(25);} 
	for(int i = 1; i<yukseklik; i++){coordinateCalculation(0,yukseklik-i); cout<<b; Sleep(25);}
	coordinateCalculation(0,yukseklik+1);
	return 0;
}
