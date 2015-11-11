# -WSQ15-Babylonian-Method
#include iostream>
#include cmath>
using namespace std;

float Babylonian (float n){

  float error=0.0001;
  
  float s=n;
  
  while ((s- n/s)>error){
  
    s =((s+n/s)/2);
    
    cout <<"The intermediate number is "<<s<<endl;
    

  }
  return s ;
}

void newline(){
  cout<<endl;
}

int main(){
    float n;
    
    cout<<"Insert for Babylonian method,  "<<endl;
    
    cout <<"please be patient... "<<endl;
    
    cin>>n;
    
    newline();
    
    float a= Babylonian(n);
    
    cout <<"The root in Babylonian method is "<< a <<endl;

 return 0;
 }
