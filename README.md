# decimal-to-binary
adding the results of deimal to binary
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int n;
    scanf("%d",&n);
    int i=0,b[100],j,c=0;
    while(n>0)
    {
        b[i]=n%8;
        n=n/8;
        i++;
    }
    for(int j=i-1;j>=0;j--)
    {
        c+=b[j];
    }
    printf("%d",c);
    return 0;
    
   }
