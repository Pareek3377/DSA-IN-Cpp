//CODE OF BS:
#include<iostream>
using namespace std;

int  binarySearch(int arr[],int size,int key){
    int start=0;
    int end=size-1;
    int mid=(start+end)/2;

    while(start <= end){
        if(arr[mid]==key){
            return mid;
        }
        if(key > arr[mid]){
            start=mid+1;
        }
        else{
            end=mid-1;
        }
        mid=(start+end)/2;
    }
    return -1;
}
int main(){
    int even[6]={1,5,3,6,17,9};
    int odd[5]={2,3,5,6,12};

    int evenindex=binarySearch(even,6,17);
     cout<<"Index of 17 is : "<<evenindex<<endl;
    int oddindex=binarySearch(odd,5,6);
    cout<<"index of 6 is : "<<oddindex<<endl;

}

//FirST AND LAST OCCURENCE OF AN ELEMENT USING BINARY SEARCH
#include<iostream>
using namespace std;

int firstOccurence(int arr[],int n,int key){
    int s=0,e=n-1;
    int mid=s+(e-s)/2;
    int ans=-1;
    while(s<=e){
        if(arr[mid]==key){   //left most occurence
            ans= mid;
            e=mid-1;
        }
        else if(key> arr[mid]){ //right me jao
            s=mid+1; 
        }
        else if(key<arr[mid]){   //left me jao
            e=mid-1;
        }
        mid=s+(e-s)/2;
    }
    return ans;
}
int lastOccurence(int arr[],int n,int key){
    int s=0,e=n-1;
    int mid=s+(e-s)/2;
    int ans=-1;
    while(s<=e){
        if(arr[mid]==key){   //left most occurence
            ans= mid;
            s=mid+1;
        }
        else if(key> arr[mid]){ //right me jao
            s=mid+1; 
        }
        else if(key<arr[mid]){   //left me jao
            e=mid-1;
        }
        mid=s+(e-s)/2;
    }
    return ans;
}
int main(){
    int even[11]={1,2,3,3,3,3,3,3,3,3,5};

    cout<<"First ooccurence of 3 is at index : "<< firstOccurence(even,11,3)<<endl;
    cout<<"last ooccurence of 3 is at index : "<< lastOccurence(even,11,3)<<endl;

}
