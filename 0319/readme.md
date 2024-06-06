디렉토리 관련 명령어
-
![image](https://github.com/mooner1213/SystemPgm/assets/162667655/55f4717c-3ece-4036-9213-a1b2ca5dbeff)



rm 명령어
-
rm [삭제 대상1] [삭제 대상2] [삭제 대상3] .....<br>
ex) rm test1.txt test2.txt test3.txt<br>

현재 위치의 모든 파일 제거<br>
ex) rm -rf *<br>

현재 위치의 .txt로 끝나는 모든 파일 제거<br>
rm *.txt<br>


cat 명령어
-
파일 내용 출력
ex) $cat [파일1]<br>

여러개의 파일 출력<br>
ex) cat [파일1] [파일2]

파일 생성 / 덮어쓰기 / 이어쓰기<br>
cat > [파일명]<br>
cat > [파일명]<br>
cat >> [파일명]<br>

more / head / tail 명령어
-
more : 하나이상의 파일이름을 받고, 각 파일의 내용을 페이지단위로 출력함.<br>

head : 파일의 앞부분(10줄)을 출력<br>

tail : 파일의 뒷부분(10줄)을 출력<br>

cp 명령어
-
$cp [파일1][파일2]<br>

파일1의 복사본 파일2를 현재 디렉토리 내에 만듦.<br>

mv 명령어
-
mv : 이름을 변경함.<br>

$mv [파일1][파일2]<br>

파일1의 이름을 파일2로 변경<br>

chmod 명령어
-
파일 or 디렉토리의 사용권한을 변경함.<br>

$ chmod [-R] 사용권한 파일<br>
-R옵션은 디렉토리 내의 모든파일 / 하위 디렉토리에 대해서도 적용됨<br>

전면처리 / 후면처리
-
전면처리 : 명령어를 입력 시, 전면에서 실행되며 명령어 실행이 끝날 때까지 기다림.<br>

후면처리 : 명령어들을 후면에서 처리, 전면에서는 다른 작업을 동시 수행<br>

ex) <br>
$ (sleep 100; echo done) &<br>
[1] 8320<br>
$ find . -name test.c -print &<br>
[2] 8325<br>
$ jobs<br>
[1] + Running ( sleep 100; echo done )<br>
[2] - Running find . -name test.c –print<br>
$ fg %작업번호<br>
$ fg %1<br>
( sleep 100; echo done )<br>
 후면처리 입출력<br>
$ find . -name test.c -print > find.txt &<br>
$ find . -name test.c -print | mail chang &<br>
$ wc < inputfile &<br>

프로세스(process)
-
실행중인 프로그램을 프로세스라고 함.<br>

각 프로세스는 유일한 프로세스 번호 PID를 가짐.<br>

ps명령어를 사용, 나의 프로세스들을 볼 수 있음.<br>

$ ps<br>
PID TTY TIME CMD<br>
8695 pts/3 00:00:00 csh<br>
8720 pts/3 00:00:00 ps<br>

$ ps u<br>
USER PID %CPU %MEM VSZ RSS TTY STAT START TIME COMMAND<br>
chang 8695 0.0 0.0 5252 1728 pts/3 Ss 11:12 0:00 -csh<br>
chang 8793 0.0 0.0 4252 940 pts/3 R+ 11:15 0:00 ps u<br>

$ ps aux<br>
USER PID %CPU %MEM VSZ RSS TTY STAT START TIME COMMAND<br>
root 1 0.0 0.0 2064 652 ? Ss 2011 0:27 init [5]<br>
root 2 0.0 0.0 0 0 ? S< 2011 0:01 [migration/0]<br>
root 3 0.0 0.0 0 0 ? SN 2011 0:00 [ksoftirqd/0]<br>
root 4 0.0 0.0 0 0 ? S< 2011 0:00 [watchdog/0]<br>
...<br>
root 8692 0.0 0.1 9980 2772 ? Ss 11:12 0:00 sshd: chang [pr<br>
chang 8694 0.0 0.0 9980 1564 ? R 11:12 0:00 sshd: chang@pts<br>
chang 8695 0.0 0.0 5252 1728 pts/3 Ss 11:12 0:00 -csh<br>
chang 8976 0.0 0.0 4252 940 pts/3 R+ 11:24 0:00 ps aux<br>
