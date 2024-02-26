class Solution {
  public:
    // Program for zig-zag conversion of array
    void zigZag(int a[], int n) {
        int temp=0;
        for(int i=0;i<n;i++){
    if(i%2!=0){
        if(a[i]<a[i-1] && i>0){
            temp=a[i];
            a[i]=a[i-1];
            a[i-1]=temp;
            
        }
             
    if(a[i]<a[i+1] && i<n-1){
         temp=a[i];
            a[i]=a[i+1];
            a[i+1]=temp;
        
    }
            
            
        
    }
    }
