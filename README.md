# 用来记录一些简单的判断数的方法

## 判断是否为整数

可以通过判断对变量取余后余数是否为零来判断，即</br>

```
#include<stdio.h>

int main()
{
    int a;
    scanf("%d", &a);
    if (a % 1 == 0) {
        printf("a是整数");
    } else{
        printf("a不是整数");
    }
    return 0;
}
```

## 判断是否为平方数

可以通过判断变量开根是否为整数来判断是否为平方数,即</br>

```

#include<stdio.h>
#include<math.h>

int main()
{
    int a;
    scanf("%d", &a);
    
    //这里在不同语言有不同的表示方法，如python就是if((a ** 0.5) % 1 == 0):
 
    if ((sqrt(a)) == (int)sqrt(a)) {
        printf("a是平方数");
    } else{
        printf("a不是平方数");
    }
    return 0;
}
```
