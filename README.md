/******************************************************************************
TO FIND MAXIMUM AND MINIMUM ELEMENT IN THE ARRAY

*******************************************************************************/
#include <iostream>

using namespace std;

int main()
{
    int n, arr[10], min, max, i;
    cout << "enter the size of element: ";
    cin >> n;
    
    cout << "enter the element of the array: " << endl;
    for(i=0; i<n; i++){
        cin >> arr[i];
    }
     
    max=arr[0];
    for(i=0; i<n; i++){
        if(max<arr[i]){
            max=arr[i];
        }
    }
    min=arr[0];
    for(i=0; i<n; i++){
        if(min>arr[i]){
            min=arr[i];
        }
    }
    cout << "the largest number is: " << max;
    cout << "the minimum element is: " << min;

    return 0;
}
