UVa 12459 -  Bees' ancestors

#include<iostream>
using namespace std;

int main(){
    long long a[100];
    a[1] = 1;
    a[2] = 2;
    for(int i = 3; i < 81; i++){
        a[i] = a[i-1] + a[i-2];
    }
    int n;
    while(cin >> n){
        if(n == 0){
            break;
        }
        else {
            cout << a[n] << endl;
        }
    }
    return 0;
}
