# Open Source Software (Linux CLI) _ 202334276 김이현

### Linux
---
리눅스는 오픈소스 유닉스 계열 OS로, 서버에서 범용적으로 사용하는 OS이다. 제어 시스템이나 모바일 시스템에서도 사용한다. 보안이 뛰어나고 안정적이며 CLI에서 실행된다.

 - CLI와 GUI의 차이

![Pictures](https://ipwithease.com/wp-content/uploads/2020/06/GUI-VS-CLI-TABLE-NEW.jpg)

---

### GIT Bash 문법
- pwd : 현재 파일 경로를 표시함
- cd : 파일 경로 변경
- ls : 현재 경로의 파일과 경로를 리스트로 표시
-- ls -l : 세부 사항 표시
-- ls -lh : unit 사이즈로 세부 사항 표시
-- 파일 표시 방법
    ----------     -------  -------  -------- ------------ -------------
        |             |        |         |         |             |
        |             |        |         |         |         File Name
        |             |        |         |         |
        |             |        |         |         +---  Modification Time
        |             |        |         |
        |             |        |         +-------------   Size (in bytes)
        |             |        |
        |             |        +-----------------------        Group
        |             |
        |             +--------------------------------        Owner
        |
        +----------------------------------------------   File Permissions
- ls의 다른 문법들
![Pictures](https://cyber.gachon.ac.kr/ubion_document/f4/d0/f4d0d90d47869136690b2ef358d6e648b94d400c/f4d0d90d47869136690b2ef358d6e648b94d400c.files/16.png)
- cp : 파일 또는 폴더 복사 ( cp [옵션][복사 할 디렉토리/파일][복사 될 디렉토리/파일] )
- mv : 파일 또는 폴더 이동 혹은 이름 변경
- rm : 파일 또는 폴더 영구 삭제 ( 영구 삭제되기에 windows 파일 탐색기에서 지우는게 나음 )
- mkdir : 새 폴더 생성
- Wildcard : 파일 명 혹은 폴더 명을 패턴 형식으로 출력하게 만들어줌
-- * : 일치되는 모든 문자열을 찾아주는 명령어
-- ? : 일치되는 모든 문자를 찾아주는 명령어
-- [] : [] 안에 있는 character들의 패턴에 일치하는 것을 찾아주는 명령어
- help 명령어
-- help : 간결히 도와주는 명령어
-- man : 세부적으로 도와주는 명령어
-- exit : 터미널 종료
