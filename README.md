# 1373A---Donut-Shops
#include <bits/stdc++.h>
using namespace std;
#define ull unsigned long long
 
int main(){
 
    int t;
    cin>>t;
    while(t--){
        int a,b,c;
        cin>>a>>b>>c;
        if(a>c){
            cout<<-1<<" "<<b<<endl;
        }else if(c>a){
            ull fprice=(ull)b*a;
            ull sprice=(ull)c;
            if(fprice<sprice){
                cout<<b<<" "<<-1<<endl;
            }else if(fprice>sprice){
                cout<<1<<" "<<b<<endl;
            }else{
                cout<<1<<" "<<-1<<endl;
            }
 
        }else{
            cout<<-1<<" "<<b<<endl;
        }
 
    }
 
}
 
