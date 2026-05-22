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
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo adduser clouduser</blockquote></details>
* **문제22** : 현재 로그인 중인 사용자 정보를 확인하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>id (또는 단순히 계정명만 확인 시: whoami)</blockquote></details>
* **문제23** : `clouduser`의 그룹 정보를 확인하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>groups clouduser</blockquote></details>
* **문제24** : `clouduser`에 `sudo` 권한을 부여하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo usermod -aG sudo clouduser</blockquote></details>
* **문제25** : `test.txt` 파일 소유자를 `clouduser`로 변경하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo chown clouduser test.txt</blockquote></details>
* **문제26** : `test.txt` 파일에 실행 권한을 추가하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo chmod +x test.txt</blockquote></details>
* **문제27** : `test.txt` 파일 권한을 확인하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>ls -l test.txt</blockquote></details>
* **문제28** : 루트 권한으로 셸에 진입하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo su -</blockquote></details>
* **문제29** : 현재 로그인 중인 사용자 목록을 확인하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>who</blockquote></details>
* **문제30** : 현재 사용자 환경변수 `PATH`를 출력하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>echo $PATH</blockquote></details>

---

### ⚙️ 4. 프로세스 및 작업 제어
* **문제31** : 현재 실행 중인 프로세스를 확인하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>ps -ef</blockquote></details>
* **문제32** : 실시간 프로세스 상태를 확인하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>top (또는 htop)</blockquote></details>
* **문제33** : `nginx` 프로세스를 검색하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>ps -ef | grep nginx</blockquote></details>
* **문제34** : PID 1234 프로세스를 종료하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>kill 1234</blockquote></details>
* **문제35** : 백그라운드로 `sleep 100` 명령을 실행하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sleep 100 &</blockquote></details>
* **문제36** : 현재 백그라운드 작업 목록을 확인하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>jobs</blockquote></details>

---

### 📦 5. 패키지 및 서비스 관리
* **문제37** : `nginx` 서비스를 설치하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo apt install nginx</blockquote></details>
* **문제38** : `nginx` 서비스 상태를 확인하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>systemctl status nginx</blockquote></details>
* **문제39** : `nginx` 서비스를 재시작하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo systemctl restart nginx</blockquote></details>
* **문제40** : `nginx` 서비스를 부팅 시 자동 실행되게 설정하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo systemctl enable nginx</blockquote></details>
* **문제41** : `nginx` 로그를 확인하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>journalctl -u nginx</blockquote></details>
* **문제42** : 실시간 로그를 확인하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>journalctl -f</blockquote></details>
* **문제43** : `app.log` 파일에서 `error` 문자열을 검색하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>grep "error" app.log</blockquote></details>
* **문제44** : 설치된 패키지 목록을 확인하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>dpkg -l</blockquote></details>
* **문제45** : 패키지 목록을 업데이트 하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo apt update</blockquote></details>
* **문제46** : 시스템 패키지를 업그레이드 하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo apt upgrade</blockquote></details>

---

### 📝 6. vi/vim 편집기 익히기
* **문제47** : `vim` 편집기를 설치하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>sudo apt install vim</blockquote></details>
* **문제48** : `hello.txt` 파일을 `vim`으로 생성하시오.
  <details><summary>정답 확인 (클릭)</summary><blockquote>vim hello.txt</blockquote></details>
* **문제49** : `vim`에서 저장 후 종료하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>명령 모드에서 :wq 입력</blockquote></details>
* **문제50** : `vim`에서 저장하지 않고 종료하세요.
  <details><summary>정답 확인 (클릭)</summary><blockquote>명령 모드에서 :q! 입력</blockquote></details>
