# Check-the-number-prime-or-not-using-function
[main.c](https://github.com/user-attachments/files/24233748/main.c)
#include <stdio.h>

void prime(int n);
int main(){
int num;
scanf("%d",&num);
prime(num);
return 0;
}
void prime(int n){
if(n<=1){
    printf("The number is not a prime.\n");
    return;
}
int i;
for(i=2;i*i<=n;i++){
    if(n%i==0){
        printf("Not a prime.\n");
        return;
    }
}
printf("Prime number.\n");
}
