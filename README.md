# 98lilchen.github.io
I am 98lilchen
# pop smoke
![下載](https://user-images.githubusercontent.com/114201493/197105787-f129285b-6c65-478a-8c84-fbd51cde2a8f.jpg)

long long int 各種類型
```cpp
#include <stdio.h>
int main()
{
    int n = 1234567812345678;
    printf("%d\n",n);

    long long int a = 1234567812345678;
    printf("%lld",a);
}
```
最大公因數
```cpp
#include <stdio.h>
int main()
{
    long long int a, b;
    scanf("%lld %lld", &a, &b);

    long long int ans;
    for(long long int i =1; i<=a; i++){
        if(a%i==0 && b%i==0) ans = i;
    }
    printf("答案是:%lld\n", ans);
}
```
long long int 最大公因數
```cpp
#include <stdio.h>
int main()
{
    long long int a, b, c;
    scanf("%lld%lld", &a, &b );

    while(1){
        c = a%b;
        printf("%lld %lld %lld\n", a, b, c);
        if(c==0) break;
        a=b;
        b=c;
    }
    printf("答案是:%lld\n", b);
}
```
剝皮法
```cpp

#include <stdio.h>
int main()
{
    int n=123456789;

    while( n>0 ){
    printf("個位數是%d\n", n%10 );
    n = n / 10;
    }
}

```

