# 🐧 Linux 기초 실습 문제 1~50 정답안

### 📁 1. 기본 디렉터리 및 파일 제어
* **문제1** : 현재 위치를 출력하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>pwd</blockquote></details>
* **문제2** : `linux-study` 디렉터리를 생성하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>mkdir linux-study</blockquote></details>
* **문제3** : `linux-study` 디렉터리로 이동하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>cd linux-study</blockquote></details>
* **문제4** : `test.txt` 파일을 생성하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>touch test.txt</blockquote></details>
* **문제5** : 현재 디렉터리 파일 목록을 숨김 파일 포함해서 출력하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>ls -al</blockquote></details>
* **문제6** : `test.txt` 파일 안에 "hello world" 내용을 저장하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>
  * 방법 1 (편집기 사용): vim test.txt -> 'i'를 눌러 입력 모드 진입 후 hello world 작성 -> ESC 누른 후 :wq 입력하여 저장 후 종료<br>
  * 방법 2 (단축 명령어): echo "hello world" > test.txt
  </blockquote></details>
* **문제7** : `test.txt` 파일 내용을 출력하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>cat test.txt</blockquote></details>
* **문제8** : `test.txt` 파일을 `backup.txt`로 복사하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>cp test.txt backup.txt</blockquote></details>
* **문제9** : `backup.txt` 파일 이름을 `newbackup.txt`로 변경하기.
  <details><summary>정답 확인 (클릭)</summary><blockquote>mv backup.txt newbackup.txt</blockquote></details>
* **문제10** : 현재 로그인한 사용자 이름을 출력하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>whoami</blockquote></details>

---

### 📂 2. 고급 파일 관리 및 검색
* **문제11** : `project` 디렉터리를 생성하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>mkdir project</blockquote></details>
* **문제12** : `project` 디렉터리 안에 `app.log` 파일을 생성하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>touch project/app.log</blockquote></details>
* **문제13** : 현재 디렉터리 구조를 확인하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>tree (또는 하위 폴더 전체 출력 시: ls -R)</blockquote></details>
* **문제14** : `newbackup.txt` 파일을 삭제하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>rm newbackup.txt</blockquote></details>
* **문제15** : `project` 디렉터리를 삭제하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>rm -r project</blockquote></details>
* **문제16** : 현재 디렉터리에서 `.txt` 파일만 검색하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>find . -name "*.txt"</blockquote></details>
* **문제17** : 시스템 전체에서 `nginx.conf` 파일을 검색하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo find / -name "nginx.conf"</blockquote></details>
* **문제18** : 현재 디렉터리의 파일 상세 정보를 출력하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>ls -l</blockquote></details>
* **문제19** : `test.txt` 파일 마지막 10줄을 출력하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>tail test.txt</blockquote></details>
* **문제20** : `test.txt` 파일 내용을 페이지 단위로 확인하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>less test.txt</blockquote></details>

---

### 👤 3. 사용자 권한 및 보안 설정
* **문제21** : `clouduser` 사용자를 생성하세요.
