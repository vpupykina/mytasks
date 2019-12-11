#include <stdio.h>
#include <string.h>
int main() {
    int temp;
    int N=8;
    int arr[8]={5,6,3,4,2,-7,6,1};
    for(int i=0; i<N-1; i++){
        for(int j=N-1; j>i; --j){
           if(arr[j]<arr[j-1])
           {
               temp=arr[j];
               arr[j]=arr[j-1];
               arr[j-1]=temp;
               
               
           }
          
        }
       
    }
for(int i=0; i<N-1; ++i){
    printf("%d\n" , arr[i] );
}
    
        return 0;
}

