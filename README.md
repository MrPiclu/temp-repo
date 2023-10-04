### I/O Redirection(입출력 방향 전환)

- Standard Output
	- ls -lh > a.txt : 출력 결과를 a.txt 파일로 저장, a.txt. 파일을 생성함
	- ls -lh >> a.txt : 출력 결과를 a.txt 파일로 저장, 만약 a.txt 파일이 이미 존재하는 경우 내용을 추가하여 저장함

- Standard Input
	- sort < words.txt > sorted_words.txt 예제
		- sort < words.txt : sorting 된 결과를 출력함
		- words.txt > sorted_words.txt : sorting 된 결과를 sorted_words.txt에 저장함
- Pipeines "|" : 앞선 커맨드의 출력을 다음 커맨드의 입력으로 가져감
	- command1 | command2 | command 3 |....
	- ls -lh | less : 원하는 만큼 스크롤 하며 데이터를 볼 수 있음

- Expansion
	- echo print out the text : echo 뒤의 print out the text를 그대로 출력함
	- echo * : 현재 디렉토리에 있는 file들을 출력함
	- echo ~ : 현재 사용자의 홈 디렉토리를 출력

- *TIP* : Backslash ("\\") : \\ 를 사용하면 다양한 명령어를 줄을 띄워서 입력 가능함
```
% ls -l \
> --reverse \
> --human-readable
```

- permissions (권한)
	- Linux is a multi-user system
	- 소유자에 따라 파일이나 디렉토리에 할당된 권한이 다름
	- rwx : Read Write eXecute
![Pictures](https://cyber.gachon.ac.kr/ubion_document/88/b1/88b161556b36f4629a466ea3a6d8652ff2b9a839/88b161556b36f4629a466ea3a6d8652ff2b9a839.files/8.png)

- Changing Permissions
![Pictures](https://cyber.gachon.ac.kr/ubion_document/88/b1/88b161556b36f4629a466ea3a6d8652ff2b9a839/88b161556b36f4629a466ea3a6d8652ff2b9a839.files/9.png)
```
6 = 110 = rw- for owner :owner가 reading write은 가능하지만 execute는 불가능함
0 = 000 = --- for group : group은 모든 권한을 가지지 않음
0 = 000 =--- for others : others는 모든 권한을 가지지 않음
```
	- words.txt란 파일의 권한을 바꿔보자!
		- chmod 644 words.txt -->
		- -rw-rw-r-- 1 youngmin youngmin   30   9월   28 14:27 word.txt 

- Superuse(Administaor)
	- sudo로 사용
	- sudo -i : root 계정으로 진입해서 계속 superuse 권한 유지됨

- Text Editors
 ![Pictures](https://cyber.gachon.ac.kr/ubion_document/88/b1/88b161556b36f4629a466ea3a6d8652ff2b9a839/88b161556b36f4629a466ea3a6d8652ff2b9a839.files/12.png)
 - vi, vim : 키보드 단축키로 대부분 작업하여 진입장벽이 높지만 널리 사용됨
 - nano : 초보자들이 쓰기에 비교적으로 편리한 툴
 - gedit, kwrite : 인터페이스가 GUI로 개인 컴퓨터에서 사용하기 유용함

- Shell Script
![Pictures](https://cyber.gachon.ac.kr/ubion_document/88/b1/88b161556b36f4629a466ea3a6d8652ff2b9a839/88b161556b36f4629a466ea3a6d8652ff2b9a839.files/13.png)
- ^O : Ctrl + O : Write Out(저장)

- *TIP* History
	- history 명령어를 사용하면 기록을 남길 수 있음
	- history > history_command.txt : 기록을 history_command.txt 파일을 생성해 저장함

