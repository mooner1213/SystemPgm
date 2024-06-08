# 프로그램 시작 / 종료

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/8fffd024-6d7f-4cbd-b8e3-9ede3d7799c8)

# 프로세스

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/f42d3812-0410-40c9-9650-5ea97fa756cb)
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/58bd6ce7-dcb8-462c-a33f-92e3c427de8a)
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/5ed15fce-e489-4fa2-9624-9ad5de775362)
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/e2fd1fef-1acd-4737-862b-e0f4761981f8)

# fork()

![image](https://github.com/mooner1213/SystemPgm/assets/162667655/cd291ee1-de0b-4cf4-a48c-27f16a25da0a)

- 자기 자신을 복제하는 함수다.<br>
- 한 번 호출 시, 두번 리턴함.<br>
- 자식 프로세스에겐 0을 리턴, 부모 프로세스에겐 자식프로세스 id를 리턴함.<br>

**fork1**
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/10448858-9d1d-4a64-aaa8-74506f44c7b8)
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/92e879ee-1529-45a6-967e-c839b8ef7684)


**fork2**
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/a3a3d5ef-797a-48a6-9521-5ec99a85e29c)
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/aa551166-ce7a-476b-b44c-dfa05deb02c8)


**fork3**
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/eb1c1883-6391-44c6-ae90-0a65f13b9a4b)
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/472761d2-f286-400f-94d0-2390e3331542)


# wait

**forkWait.c**
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/06f79970-2fa1-4138-93d0-053e26cec224)

**waitPid.c**
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/b8a268fc-fbc2-4fb6-a8fd-f8f138422302)

# exec
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/344589cc-15f7-4678-af04-43a79ce86ff1)

**exec1.c**
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/013d9f36-3be3-4502-b612-0920f8ab8728)

**exec2.c**
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/29cff15e-d5f8-4016-9f19-86db9d586a6a)

**exec3.c**
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/df2425d6-9d44-4517-898f-07ac69d55865)

**systemTest.c**
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/7d0de4a5-ecda-4be9-9aaf-5840c3be4c19)

**system.c**
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/cbbf6df5-a60e-45a2-bd2e-33747e2557fd)

**systemCall.c**
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/165fdb29-fc63-4c64-a274-4364c1f97111)
