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

## 判断是否为素数

用数学的方法可以证明，不能被2~sqrt(m)（取整）之间的整数整除的数，一定不能被1和他本身之外的其他任何整数整除，故可以根据这个定义来写函数</br>

```
int isPrime(int n){
	//1不是素数，所以要先判断传入的参数是否为1 
	if(n==1){
		//如果为1则返回0 
		return 0;
	}else{
		//sqrt()函数需要cmath头文件 
		for(int i=2;i<=sqrt(n);i++){
		if(n%i==0){
			return 0;
		}
	}
	//没有在2~m-1之间找到n的商，证明此数是素数，返回1 
	return 1;
	}
	
}
```
