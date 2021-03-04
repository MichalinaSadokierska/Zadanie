//Napisz program, który wczytuje ze standardowego wejścia trzy liczbycałkowite i wypisuje na standardowym
//wyjściu największą z ich wartości (pamiętaj o przypadku gdy wszystkie podane liczby lubdwiez nich są równe).
#include <iostream>
#include <string>
using namespace std;

int main()
{
int a,b,c,najwieksza;
cout << "Podaj trzy liczby calkowite: ";
cin>> a >> b >> c;
    if (a > b)
    if (a > c)
    najwieksza = a;
else
    najwieksza = c;
else
    if (b > c)
    najwieksza = b;
else
    najwieksza = c;
cout<<"Najwieksza liczba wynosi: "<< najwieksza<<endl;
return 0;
}

//Napisz program, który wczytuje ze standardowego wejścia współczynniki równania kwadratowego z jedną
//niewiadomą i wypisuje nastandardowym wyjściu wszystkie rozwiązania rzeczywiste tego równanialub odpowiednią
//informację w przypadku braku rozwiązań.
#include <iostream>
#include <string>
using namespace std;

int main()
{
int a, b, c, x1, x2, x0, delta;
cout<<"Podaj trzy liczby wspolczynniki a,b,c: ";
cin>> a >> b >> c;
delta = b*b - 4*a*c;
    if(delta>0)
{
    delta = (delta);
    x1 = (-b - delta)/(2*a);
    x2 = (-b + delta)/(2*a);
cout<<"Sa dwa pierwiastki rownania: "<<x1<<" "<<x2;
}
else
    if(delta==0)
{
    x0 = -b/(2*a);
cout<<"Jest jeden pierwiastek: "<<x0;
}
else
cout<<"Brak pierwiastkow";
return 0;
}

//Napisz program kalkulator, który wykonuje wybraną przez użytkow-nika operacją arytmetyczną na dwóch
//wczytanych liczbach. Programpowinien wczytywać dane ze standardowego wejścia i wypisywać wynik na
//standardowym wyjściu.
#include <iostream>
#include <string>
using namespace std;

int main()
{
int a, b;

cout << "Podaj pierwsza liczbe: ";
cin >> a;

cout << "Podaj druga liczbe: ";
cin >> b;

cout << a << " + " << b << " = " << a+b <<endl;

cout << a << " - " << b << " = " << a-b <<endl;

cout << a << " * " << b << " = " << a*b <<endl;

cout << a << " / " << b << " = " << a/b <<endl;

return 0;
}

//Napisz program, który wczytuje ze standardowego wejścia nieujemną liczbę całkowite wypisuje na standardowym
//wyjściu sumę kwadratów liczb od 0 do n, czyli wartość 02+ 12+ 32+...+n2.
#include <iostream>
#include <string>

int main()
{
int n, suma=0;
std::cin >> n;
while(n)
suma+=n*n--;
std::cout << suma;
return 0;
}
