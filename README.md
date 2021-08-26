# zoho.c
An interview question
#include <stdio.h>

int main()
{
    int a[]={10,1,-4,-10,9,-1,4,-9},i,j,c=0;
    for(i=0;i<8;i++) {
        for(j=i+1;j<8;j++){
            if(a[i]>a[j]) {
                c=a[i];
                a[i]=a[j];
                a[j]=c;
                
            }
        }
    }
       for(i=0;i<4;i++){
           for(j=i+1;j<4;j++){
            if(a[i]<a[j]) {
                c=a[i];
                a[i]=a[j];
                a[j]=c;
                
            }
        }
       }
       for(i=0;i<8;i++){
           printf("%d\t",a[i]);
       }
}
