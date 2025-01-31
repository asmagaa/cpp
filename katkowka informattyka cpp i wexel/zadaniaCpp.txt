//Zad 1:
#include <iostream>
using namespace std;

int main() {
    int x;
    cout << "Podaj liczbe calkowita";
    cin >> x;

    while (i <= x) {
        if (i % 2 == 0) {
            cout << i << " ";
        }
        i++;
    }
    return 0;
}

//Zad 2:
#include <iostream>
using namespace std;

int main() {
    int x;
    int suma = 0;
    int i = 1;
    cout << "Podaj liczbe calkowita: ";
    cin >> x;

    while (i <= x) {
        suma += i;
        i++;
    }

    cout << "Suma liczb od 1 do: " << x << " wynosi: " << suma << endl;
} */

// Zad 3:
#include <iostream>
using namespace std;

int main() {
	int x, y;
	int iloczyn = 0;
	int i = 0;
	cout << "Podaj dwie liczby calkowite: ";
	cin >> x;
	cin >> y;

	while (i < y) {
		iloczyn += x;
		i++;
	}
	cout << "Iloczyn " << x << " i " << y << " wynosi: " << iloczyn << endl;
}

// Zad 4:
#include <iostream>
using namespace std;

int main() {
    int x;
    int i = 2;
    bool pierwsza = true;
    cout << "Podaj liczbe calkowita: ";
    cin >> x;
    
    while (i <= x / 2) {
        if (x % i == 0) {
            pierwsza = false;
            break;
        }
        i++;
    }
    
    if (pierwsza && x > 1) {
        cout << x << " jest liczba pierwsza." << endl;
    } else {
        cout << x << " nie jest liczba pierwsza." << endl;
    }
    return 0;
}

// Zad 5:
#include <iostream>
using namespace std;

int main() {
    int n, silnia = 1, i = 1;
    cout << "Podaj liczbe calkowita: ";
    cin >> n;

    while (i <= n) {
        silnia *= i;
        i++;
    }
    cout << "Silnia z " << n << " wynosi: " << silnia << endl;
    return 0;
}

// Zad 6:
#include <iostream>
using namespace std;

int main() {
    int n;
    cout << "Podaj liczbe calkowita: ";
    cin >> n;

    if (n == 0) {
        cout << "Odwrotnosc z 0 nie istnieje." << endl;
    } else {
        cout << "Odwrotnosc liczby " << n << " wynosi: " << 1.0 / n << endl;
    }
    return 0;
}

// Zad 7:
#include <iostream>
using namespace std;

int main() {
    int n, suma = 0, i = 1;
    cout << "Podaj liczbe calkowita: ";
    cin >> n;

    while (i < n) {
        if (n % i == 0) {
            suma += i;
        }
        i++;
    }
    
    if (suma == n) {
        cout << n << " jest liczba doskonala." << endl;
    } else {
        cout << n << " nie jest liczba doskonala." << endl;
    }
    return 0;
}

// Zad 8:
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cout << "Podaj dwie liczby calkowite: ";
    cin >> a >> b;

    double srednia = (a + b) / 2.0;
    
    cout << "Srednia arytmetyczna " << a << " i " << b << " wynosi: " << srednia << endl;
    return 0;
}

// Zad 9:
#include <iostream>
using namespace std;

int main() {
    int n;
    cout << "Podaj liczbe calkowita: ";
    cin >> n;

    int i = 0;
    
    while (i * i <= n) {
        i++;
    }
    cout << "Pierwiastek kwadratowy z " << n << " wynosi w przyblizeniu: " << i - 1 << endl;
    return 0;
}

#include <iostream>
using namesopace std;

int main(){
	double n, guess, epsilon = 0.000001;
	cin>>n;
	guess = n;
	while((guess*guess-n)>epsilon){
		guess = (guess+n/guess)/2;
	}
	return guess;
