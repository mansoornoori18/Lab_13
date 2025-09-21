#include <iostream>  // COMSC-210 | Lab 12 | Mansoor Noori
#include <array>     // IDE Visual Studio,
#include <fstream>   // for file input&output

// to vaoid using std through out the project
using namespace std;

int main(){

    // create an array to hold the stock quantity 
    array<int, 30> stock{};

    // open the file that contain the stock numbers 
    ifstream file("inventory.txt");

    // check if the file opened succefully 
    if (!file) {
        cout << "could not open inventory.txt\n";
        return 1;
    }
    // read all stock quantities from file 
    for (size_t i = 0; i < stock.size(); i++){
        file >> stock[i];
    }
    // Display stock 
    cout << "Store inventory (quantities):\n";
    for ( int qty : stock){
        cout << qty <<" ";
    }
    cout << "\n";

    //std::array functions to display array info
    cout << "\n--- Array Info ---\n";
    cout << "Total items: " << stock.size() << "\n";               // .size()
    cout << "First item stock: " << stock.front() << "\n";         // .front()
    cout << "Last item stock: " << stock.back() << "\n";           // .back()
    cout << "Item at index 5 has stock: " << stock.at(5) << "\n";  // .at()
    
    // Use .fill() to reset all stock values to 0
    stock.fill(0);

    // Print array after fill
    cout << "\nAfter resetting stock (fill(0)):\n";
    for (int qty : stock){
        cout << qty << " ";
    }
    cout << "\n";
    
    return 0;
}