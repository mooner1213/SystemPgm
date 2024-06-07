# 파일시스템 구조

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/f88f3b22-22d5-455d-a417-18030ec03da9)

**부트블록**<br>
- 파일 시스템 시작부에 위치, 보통 첫번째 섹터를 차지함.<br>
- 부트 스트랩 코드가 저장되는 블록이다.<br>

**슈퍼블록**<br>
- 전체 파일 시스템에 대한 정보 저장.<br>
 *총 블록 수, 사용가능한 i-node 개수, 등<br>

**i-list**<br>
- 각 파일을 나타내는 모든 i-node들의 리스트<br>
- 한 블록은 약 40개의 i-node를 포함<br>

**데이터 블록**<br>
- 파일의 내용을 저장하기 위한 블록들<br>

**i-node**<br>
- **한 파일은 하나의 i-node를 갖는다.** <br>
- 파일에 대한 모든 정보를 가지고 있다.<br>
  * 파일타입 : 일반 파일, 디렉토리, 블록 장치, 문자 장치 등<br>
  * 파일크기<br>
  * 사용권한<br>
  * 파일 소유자 및 그룹<br>
  * 접근 및 갱신 시간<br>
  * 데이터 블록에 대한 포인터<br>

  # 블록 포인터

  ![image](https://github.com/mooner1213/SystemPgm/assets/162667655/5fc7db29-5c4c-4d75-a5f8-7a6f6eb9f345)
  ![image](https://github.com/mooner1213/SystemPgm/assets/162667655/ca5d50dc-5f55-495c-b714-99831968581d)

# ftype.c

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/0bfa3dda-80e7-4af1-b4c8-b4288f80f0d3)

# chmod(), fchmod()

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/2349725b-c3c2-4d39-902b-c3e69fce6ec9)<br>

**fchmod.c**<br>

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/192cd11d-a20a-4ee6-b063-026c6359d22f)

# cptime.c

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/e92f02c8-3e76-4188-9afc-9f08e6948f93)
