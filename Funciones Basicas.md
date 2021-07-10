- 👋 Hi, I’m @wes343
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

#include <iostream>
#include <stdlib.h>
#include <math.h>

using namespace std;

//Funciones

int suma(int a, int b) 
{
	int r = 0;
	r = a + b;
	return r;
}
int producto(int a, int b)
{
	int r = 0;
	r = a * b;
	return r;
}
int cubo (int a)
{
	int c = 0;
	c = pow(a, 3);
	return c;
}
int main()
//Programa con menu de funciones que sume, multiplique y que calcule el valor de un cubo
{
	int numero_1, numero_2,opcion_User, x = 0;
	do {
		system("cls");
		cout << "************MENU DE OPCIONES***********" << "\n";
		cout << "	1- Sumar					    		" << "\n";
		cout << "	2- Multiplicar						" << "\n";
		cout << "	3- Cubo							    	" << "\n";
		cout << "	4- Salir							    " << "\n";
		cout << "***************************************" << "\n";
		cout << endl;
		cout << "Digita tu opcion: ";
		cin >> opcion_User;
		switch (opcion_User)
		{
		case 1:
			cout << "Introduce el primer numero: ";
			cin >> numero_1;
			cout << "Introduce el segundo numero: ";
			cin >> numero_2;
			cout << "La suma de los dos primeros numeros es: " << suma(numero_1, numero_2) << endl;
			break;
		case 2:
			cout << "Introduce el primer numero: ";
			cin >> numero_1;
			cout << "Introduce el segundo numero: ";
			cin >> numero_2;
			cout << "El producto de los dos numeros es: " << producto(numero_1, numero_2) << endl;
			break;
		case 3:
			cout << "introduce el valor: ";
			cin >> numero_1;
			cout << "El cubo es: " << cubo(numero_1) << endl;
			break;
		case 4:
			cout << "----------Saliendo----------" << endl;
			x = 4;
			break;
		default:
				cout << "Opcion no disponible" << endl;
		}
		system("pause");
	} while (x != 4);
	
	return 0;
}
