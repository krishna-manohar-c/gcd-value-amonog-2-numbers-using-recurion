# gcd-value-amonog-2-numbers-using-recurion
#include<stdio.h>
int gcd(int a, int b){
if(b==0){
return a;
}
else{
return gcd(b,a%b);
}
}
int main(){
int a,b;
printf("enter two numbers:\n");
scanf("%d %d",&a,&b);
gcd(a,b);
printf("GCD of two numbers %d and %d : %d",a,b,gcd(a,b));
return 0;
}


