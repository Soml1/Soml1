#include <iostream>

using namespace std;
int main()
{
    int x = 0;
    int mx = 0 ;
    int o[9];
    int y=0;
    int tab[9];
    cout << "Podawanie liczb-1 " << "Wylosuj losowe liczby-2" << endl;
    cin >> x;
    cout << endl;
    if (x==1) {
        cout << "Prosze podac dziesiec liczb" << endl;
        cin >> o[0] >> o[1] >> o[2] >> o[3] >> o[4] >> o[5] >> o[6] >> o[7] >> o[8] >> o[9];
        for (int i = 0;i < 10; i++) {
            if (o[i] > mx){
                mx = o[i];

        }

    }
 cout << "naj to: " << mx;
    }

    if (x==2) {
        //while (y<10){
            for (int i = 0;i < 10; i++) {
                int r = rand();
                tab[i] = r;
                cout << tab[i] << endl;
                //if (r<99 && r>1){
                //    tab[i] = r;
                //    cout << tab[i] << endl;
                //    y++;
                //}
            }
    //}
    for (int i = 0;i < 10; i++) {

    if (tab[i] > mx){
        mx=tab[i];

    }

    }
    cout << "naj to: " << mx;
    }
    return 0;
}
