# Additive-pesitence-multiplicative-persistence
Additive persistence And Multiplicative persistence
//C++
#include<iostream>
using namespace std;
int main()
{
    int sum=0,n,r=0,s=0,nn,ss=1,p=1,pp=0;
    cout<<"ENTER NUMBER--";
    cin>>n;
    int t=n;
    while(n!=0)
    {
        r=n%10;
        sum=sum+r;
        n=n/10;
    }
    nn=sum;
    while(nn!=0)
    {
        r=nn%10;
        s=s+r;
        nn=nn/10;
    }
    while(t!=0)
    {
        r=t%10;
        ss=ss*r;
        t=t/10;
    }
    pp=ss;
    while(pp!=0)
    {
        r=pp%10;
        p=p*r;
        pp=pp/10;
    }
    cout<<"\nSUM OF NUMBER--"<<sum;
    cout<<"\nADDITIVE--"<<s;
    cout<<"\nMULTIPLICATION--"<<ss;
    cout<<"\nMULTIPLICATIVE--"<<p;
    return 0;
}
