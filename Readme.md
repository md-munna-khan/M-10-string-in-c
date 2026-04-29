# M-10 string in c

![alt text](image.png)

# 10-2 What is string
- space " " is also a character
![alt text](image-1.png)

- now its okay 
![alt text](image-2.png)

## 10-3 String input and output

- string special power

![alt text](image-3.png)

- after input receive then compiler receive null value thats why compiler output is stop

![alt text](image-4.png)

## 10-4 Null character
- scanf when in string under input receive space he can not received 
```c
#include<stdio.h>
int main()
{
    char s[10];
    scanf("%s",&s);
    printf("%s\n",s); 
  
    return 0;
}
```

![alt text](image-5.png)

## 10-5 String input with space

- scanf is not receive properly our long string value  ❌
![alt text](image-6.png)

- we can use gets but this is not standard way 

![alt text](image-7.png)

-   fgets also enter he can receive as a input 
```c
#include <stdio.h>
int main()
{
    char s[50];
    // gets(s);
    // fgets(s,size,standard input )
    // fgets(s,3,stdin);
    // scanf("%s",s);
    printf("%s", s);
    return 0;
} 
```

![alt text](image-8.png)

## 10-7 String initialization

- initialization normal way

```c
  #include<stdio.h>
  int main()
  {
      char s[6]={'m','u','n','n','a'};
      printf("%s",s);
      return 0;
  }     
 ```

- super power
```c
  #include<stdio.h>
  int main()
  {
    //   char s[6]={'m','u','n','n','a'};
    char s[6]="munna";
    // with space 
        char s[30]="munna mia ";
      printf("%s",s);
      return 0;
  }     
 ```
 ![alt text](image-9.png)

 ## 10-9 Length of a string

 ```c
 #include<stdio.h>
int main()
{
    char s [100];
    scanf("%s",s);
    int count=0;
    for(int i=0;s[i] != '\0'; i++)
    {
        count ++;
    }
    printf("%d",count);
    return 0;
}
```

![alt text](image-10.png)

## 10-11 Length of a string using strlen

```c
#include<stdio.h>
int main()
{
    char s [100];
    scanf("%s",s);
 int size = strlen(s);
 printf("%d",size);
    return 0;
}
```

## 10-12 Lets use getline