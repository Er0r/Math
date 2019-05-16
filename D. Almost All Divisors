#include<bits/stdc++.h>
using namespace std;

vector<int>v;
int arr[3001000];

int main()
{
    int t;
    cin>>t;
    while(t--)
    {
        v.clear();
        long long  n,k=0,l=INT_MAX;
        cin>>n;
        memset(arr,0,sizeof(arr));
        for(int i=0;i<n;i++)
        {
            long long  a;
            cin>>a;
            arr[a]=1;
            v.push_back(a);
            k=max(k,a);
            l=min(l,a);
        }
        long long num=k*l;
        int counter=0;

        for(long long i=2;i*i<=num;i++)
        {
            if(num%i==0)
            {
                if(arr[i]==0||arr[num/i]==0)
                {
                    counter=1;
                    break;
                }
            }
        }

        for(int i=0;i<n;i++)
        {
            if(num%v[i])
            {
                counter=1;
                break;
            }
        }
        if(counter)cout<<-1<<endl;
        else cout<<num<<endl;
    }
}
