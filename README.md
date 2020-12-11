#include <iostream>
#include <string>
#include <vector>
#include <algorithm>

using namespace std;

/**
 * Auto-generated code below aims at helping you parse
 * the standard input according to the problem statement.
 **/

int main()
{
    int N,i,j,k;
    int P[10000000]={0};
    int m1=P[0];
    int m2=P[0];
    int answer=m1-m2;
    cin >> N; cin.ignore();
    cin >> P[i]; cin.ignore();
   for(i=1;i<1000000;++i)
   {
       if(m1<P[i])
       {m1=P[i];
       }
       cout<<m1<<endl;
   }
   for(i=1;i<1000000;++i)
   {
    if(m2<P[i])
       {m2=P[i]&&m2<m1;
       }
       cout<<m2<<endl;
   }
   cout<<answer<<endl;
   return 0;
}
