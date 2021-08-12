# pp5-1
// Example program
//incluye < iostream >
//usando el espacio de nombres std;

// Correccion de los cinco errores.
#include <iostream>
using namespace std; 

int  main () 
{

 int n,aux;
cout<<"Ingrese la cantidad de numeros :";
 cin>>n;
 
 int V[n];
 for( int i=0;i<n;i++) {
  cout<<"\n Numero "<<i+1<<" = ";
  cin >>V[i];
  }
  
//Algoritmo de la Burbuja
 for(int i=0;i<n;i++){
  for ( int j=i+1;j<n;j++) {
   if (V [j] <V [i]) {
    aux = V [i];
    V [i] = V [j];
    V [j] = aux;
    
   }
  }
 }

//Procedemos a imprimir los resultados ordenados
cout << " Elementos Ordenados: " << endl;
 for( int i = 0 ; i <n; i ++) {
  cout << V [i] << endl;
 }

 return  0 ;
}
