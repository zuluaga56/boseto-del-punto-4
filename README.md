# boseto-del-punto-4
boseto del punto 4 menu
#include<string>
#include <iostream>
#include<stdlib.h>
#include "Listas4.h"

using namespace std;
/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char** argv) {
	int opc, inser;
	struct nodo * cabeza;
	struct informacion dato;
	system("color 5F");
	cabeza=crearCabeza();
	
	while(opc!=4)
	{
		cout<<"\n--PRACTICA LISTAS--";
		cout<<"\n*OPCIONES:"<<endl;
		cout<<"\n1) Opcion 1 para insertar informacion de estudiantes";
		cout<<"\n2) Opcion 2 para mostrar lista";
		cout<<"\n3) Opcion 3 para ordenar por carnet";
		cout<<"\n4) opcion 4 para ver cuantos estudiantes tienen bonificaciones"<<endl;
		cout<<"\nIngrese la opcion:";cin>>opc;
		switch(opc)
		{
			case 1: 
						cout<<"\nIngrese (1) si desea insertar por el inicio o (2) si desea insertar por el final: "; cin>>inser;
						if(inser=1){
						cout<<"Ingrese Carnet Nota y Bonificacion =========> "<<endl; cin>>dato.carnet>>dato.nota>>dato.bonificacion;
						insertarInicio(cabeza, dato); 
						}else{
							cout<<"Ingrese Cedula Nombre Y la Nota=========> "<<endl; cin>>dato.carnet>>dato.nota>>dato.bonificacion;
							insertarFinal(cabeza,dato);
							
						}
				break;
			case 2: 
						mostrarLista(cabeza);
				break;
				default:
				cout<<"Opcion invalda, ingrese otra opcion por favor";
		}
	
	
}
}
000
