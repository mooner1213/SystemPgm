vi 사용법
-

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/23dca6f5-5f57-4c1b-8ea8-c211eb1cbf6f)<br>

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/7c3e9eac-6355-4b1c-aa30-337cd467dfd4)<br>

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/291356ce-93f0-4e37-8538-0a460f7714a1)<br>

# gcc컴파일러<br>

-$ gcc[-옵션]파일<br>

컴파일<br>
$ gcc long.c<br>
$ a.out // 실행파일<br>


# 단일 모듈 프로그램 : long.c<br>

```
#include <stdio.h>
#include <string.h>
#define MAXLINE 100

void copy(char from[], char to[]);

char line[MAXLINE];
char longest[MAXLINE];

int main(){
        int len;
        int max;
        max = 0;
        while (gets(line) != NULL){
                len = strlen(line);
                if (len > max){
                        max = len;
                        copy(line, longest);
                }
        }
        if (max > 0)
                printf("%s", longest);

        return 0;
}
```
<b>long.c</b><hr>

```
#include <stdio.h>
#include <string.h>
#include "copy.h"

char line[MAXLINE]; // 입력 줄
char longest[MAXLINE]; // 가장 긴 줄
/* 입력 줄 가운데 가장 긴 줄 프린트 */

int main(void){
        int len;
        int max;
        max = 0;
        while (gets(line) != NULL) {
                len = strlen(line);
                if (len > max){
                        max = len;
                        copy(line, longest);
                }
        }
        if (max > 0) // 입력 줄이 있었다면
                printf("%s", longest);

        return 0;
}
```
<b>main.c</b><br>
```
#include <stdio.h>
#include "copy.h"

/* copy: from을 to에 복사; to가 충분히 크다고 가정 */

void copy(char from[], char to[]){
        int i;
        i = 0;
        while ((to[i] = from[i]) != '\0')
                ++i;
}
```
<b>copy.c</b><br>

```
#define MAXLINE 100
void copy(char from[], char to[]);
```

# make 시스템

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/fadc5fef-eda0-4307-a60b-a4c78bd3c9ef)<br>

구성<br>
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/0d331738-6d80-4b03-9792-1cad3b1cf003)
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/784b3b80-6b05-4278-986f-fd9458156630)
