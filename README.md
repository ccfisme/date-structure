# 循环队列  

* 判断插入变量e后队列是否为满用的是`尾指针加一对总空间取余，看值是否为头指针`的方法  

![image](https://user-images.githubusercontent.com/74129445/145961231-f8ddc16d-a6a5-4574-a172-29ef7e796ba4.png)  
 
![image](https://user-images.githubusercontent.com/74129445/145960914-1463739b-6dcc-421d-95de-1590640efe79.png)  

这种方法变式到了从队列删除数，求最后剩的是谁  

![image](https://user-images.githubusercontent.com/74129445/145961614-c184a744-6c1b-460d-a225-8bd9ad653885.png)  

可以看到，解题的步骤用的也是对整个队列长度取余来确定上一次的循环没结束并连接到下一次循环的计数
