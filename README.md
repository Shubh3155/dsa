# dsa
1.largest element in an array
int largest(int arr[], int n) {
    // Code Here
    int largest = arr[0];
    for(int i = 0; i<n ; i++){
        if(arr[i]>largest){
            largest = arr[i];
        }
    }
    return largest;
}


2. second largest element in array
   class Solution {
  public:
    // Function returns the second
    // largest elements
    int getSecondLargest(vector<int> &arr) {
        // Code Here
        int n = arr.size();
        int largest = -1;
        int sec_largest = -1;
        for(int i = 0 ; i < n ; i++){
            if(arr[i]>largest){
                sec_largest = largest;
                largest = arr[i];
            }
            if(arr[i]<largest && arr[i]>sec_largest){
                sec_largest = arr[i];
            }
        }
        return sec_largest;
    }






