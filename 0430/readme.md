# 디렉토리 구현

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/324efabe-09b5-4551-b379-eb35b042336d)
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/f5725532-1cd6-4b53-8066-975df7b17954)

**디렉토리 리스트**<br>

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/836a9380-47c8-4b65-bc24-c666c215c691)

**list1.c**<br>
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/b95c07af-7b6b-404d-89db-773f07ec87df)

**list2.c**<br>
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/e5fd9990-3462-4124-862b-ba5bbe76225c)
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/5f8f1e6d-1656-408a-9176-c7f009dc31db)
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/08e5698b-b94d-44ce-91aa-aa12544cd9ea)

**디렉토리 만들기**<br>

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/f738cbdc-f21a-4bd5-9a8d-bbec1f4f5a75)

**디렉토리 삭제**<br>

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/3b63ec7e-cc67-4992-ad8d-ce4950df32b4)

# 링크

- 링크는 기존 파일에 대한 또 다른 이름으로, 하드링크와 소프트링크가 있다.<br>

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/2422d32b-e42d-4d8d-b358-79cee72f3802)
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/a085e297-ca9a-4d97-9bbf-9641273d2a4c)

**하드 링크 / 소프트 링크**<br>

- 하드 링크<br>
  * 파일시스템 내의 i-node를 가리킴.<br>
  * 같은 파일 시스템 내에서만 사용가능.<br>
 
- 소프트 링크<br>
  * 실제 파일의 경로명을 저장하고있는 링크.<br>
  * 파일에 대한 간접적인 포인터 역할.<br>
  * 다른 파일시스템 파일도 링크 가능.<br>

**link.c / unlink.c**

- link.c<br>
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/6fc83f03-229a-4e0a-ad1c-3f0875e55875)

- unlink.c<br>
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/ed413dba-65e1-42c3-ba95-e7815beef631)

