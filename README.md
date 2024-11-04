#include <stdio.h>

int searchElement(int *arr, int size, int key) {
    for (int i = 0; i < size; i++) {
        if (*(arr + i) == key) {
            return i; // Return the index if found
        }
    }
    return -1; // Return -1 if not found
}

int main() {
    int size;
    printf("Enter the size of the array: ");
    scanf("%d", &size);
    int arr[size];
    printf("Enter the elements of array:\n");
    for (int i=0;i<size;i++)
    {
        scanf("%d",&arr[i]);
    }
    int key;

    printf("Enter the element to search: ");
    scanf("%d", &key);

    int index = searchElement(arr, size, key);

    if (index != -1) {
        printf("Element %d found at index %d.\n", key, index);
    } else {
        printf("Element %d not found in the array.\n", key);
    }

    return 0;
}



2ND APPROACH WHERE YOU SEE MORE KEY VALUE THERE OR NOT.


