- 👋 Hi, I’m @Ayesha-Noor-1
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Ayesha-Noor-1/Ayesha-Noor-1 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
#include<iostream>
using namespace std;
int main(){
     int minindex=0,maxindex=0, summin=0,summax=0;

    int arr[5];
   
   for(int i=0; i<5 ; i++){
       cin>>arr[i];
   }
   int  min=arr[0],max=arr[0];
    for(int i=1; i<5 ;i++)
    {
        if(min>arr[i])
        {
            min =arr[i];
            minindex=i;
        }
        if(max<arr[i])
        {
            max=arr[i];
            maxindex=i;
        }
    }
   for(int i=0;i<5;i++)
   {
       if(i==maxindex)
       {
           continue;
       }
       
     else{
         
       
       summin +=arr[i];
     } 
   }
   for(int i=0;i<5;i++)
    {
    
       if(i==minindex)
       {
           continue;
    }
    else {
    
    
    summax +=arr[i];
    }
   }
   cout<<summin<<" "<<summax;
    return 0;
}
