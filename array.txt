//C Program to find the largest and smallest element in an array
#include<stdio.h>

int main(){
    int arr[100], i, n, largest, smallest;

    printf("Enter the size of the array: ");
    scanf("%d", &n);

    printf("Enter the elements: ");
    for(i=0; i<n; i++){
        scanf("%d", &arr[i]);
    }

    largest = arr[0];
    for(i=0; i<n; i++){
        if(arr[i]>largest){
            largest = arr[i];
        }
    }
    printf("Largest Value = %d\n", largest);

    smallest = arr[0];
    for(i=0; i<n; i++){
        if(arr[i]<smallest){
            smallest = arr[i];
        }
    }
    printf("Smallest Value = %d", smallest);

    return 0;
}
