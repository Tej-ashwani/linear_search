# linear_search
#include <iostream>
using namespace std;

bool search(int arr[], int size, int key) {
    for (int i = 0; i < size; i++) {
        if (arr[i] == key) {
            return true;
        }
    }
    return false;
}

int main() {
    int arr[10];
    int size;
    int key;

    cout << "Enter size of array: ";
    cin >> size;

    cout << "Enter elements of array: ";
    for (int i = 0; i < size; i++) {
        cin >> arr[i];
    }

    cout << "Enter key to search: ";
    cin >> key;

    bool found = search(arr, size, key);
    if (found) {
        cout << "Element is present." << endl;
    } else {
        cout << "Element is not present." << endl;
    }

    return 0;
}
