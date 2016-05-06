# tarea_nodo
//============================================================================
// Name        : nodos.cpp
// Author      : santiago
// Version     :
// Copyright   : 
// Description : Hello World in C++, Ansi-style
//============================================================================

#include <iostream>
#include <stdlib.h>
using std::cout;
using std::cin;
using std::endl;
struct numero{
	int informacion;
	struct numero *siguiente;
};
main(){
	struct numero *tope;
	struct numero *nuevo;
	struct numero *auxiliar;
	tope=NULL;
	int dato;
	int cantidad;
	int i=0;
	cout<<"ingrese la cantidad de numeros"<<endl;
	cin>>cantidad;
	while(i<cantidad){

		nuevo=(struct numero *)malloc(sizeof(struct numero));
	nuevo->siguiente=tope;
	cout<<"ingrese el dato"<<endl;
	cin>>dato;
	nuevo->informacion=dato;
	tope=nuevo;//
		i++;
	}
while(nuevo!=NULL){
	cout<<nuevo->informacion<<",";
	nuevo=nuevo->siguiente;
}
system("PAUSE");

}
