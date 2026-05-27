# 🐧 Linux 기초 실습 문제 

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


---

### 🧠 7. 개념 암기형
* **문제51** : 리눅스에서 Shell의 역할은 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  사용자가 입력한 명령어를 해석하여 커널에게 전달하고 결과를 출력하는 인터페이스 역할입니다.
  </blockquote>
  </details>

* **문제52** : 리눅스 최상위 디렉터리는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  루트 디렉터리 (`/`)
  </blockquote>
  </details>

* **문제53** : 파일 권한 rwx 중 `x` 권한의 의미는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  `x`는 실행 권한을 의미합니다. (참고: `r`은 읽기, `w`는 쓰기)
  </blockquote>
  </details>

* **문제54** : `/etc/passwd` 파일에는 어떤 정보가 저장되나요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  사용자 계정 정보
  </blockquote>
  </details>

* **문제55** : 심볼릭 링크와 가장 비슷한 윈도우의 개념은 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  바로가기 아이콘
  </blockquote>
  </details>

* **문제56** : 프로세스(Process)란 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  메모리에 올라와 실행 중인 프로그램을 의미합니다.
  </blockquote>
  </details>

* **문제57** : APT가 dpkg보다 편리한 가장 큰 이유는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  의존성 문제를 자동으로 해결해 주기 때문입니다.
  </blockquote>
  </details>

* **문제58** : systemd의 주요 역할은 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  서비스(데몬) 및 서비스 상태 관리
  </blockquote>
  </details>

* **문제59** : 마운트(Mount)의 의미는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  물리적인 디스크(저장장치)를 리눅스의 특정 디렉터리에 연결하는 작업입니다.
  </blockquote>
  </details>

* **문제60** : LVM(Logical Volume Manager)의 가장 큰 장점은 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  디스크 용량을 유연하게 확장 및 축소할 수 있다는 점입니다.
  </blockquote>
  </details>

---

### ⌨️ 8. 명령어 기억형
* **문제61** : 현재 작업 중인 디렉터리의 절대 경로를 확인하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  pwd
  </blockquote>
  </details>

* **문제62** : 숨김 파일을 포함하여 디렉터리의 상세 목록을 확인하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  ls -al
  </blockquote>
  </details>

* **문제63** : 현재 로그인한 사용자 계정을 확인하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  whoami
  </blockquote>
  </details>

* **문제64** : 파일이나 디렉터리의 권한을 변경하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  chmod
  </blockquote>
  </details>

* **문제65** : 파일이나 디렉터리의 소유자 및 소유 그룹을 변경하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  chown
  </blockquote>
  </details>

* **문제66** : 시스템에서 실행 중인 전체 프로세스의 상세 상태를 확인하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  ps -ef
  </blockquote>
  </details>

* **문제67** : 현재 80번 포트를 사용하고 있는 프로세스를 확인하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo lsof -i :80
  </blockquote>
  </details>

* **문제68** : Nginx 서비스를 재시작하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  systemctl restart nginx
  </blockquote>
  </details>

* **문제69** : 시스템 로그를 실시간으로 확인(모니터링)하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  journalctl -f
  </blockquote>
  </details>

* **문제70** : 시스템 내에서 파일이나 디렉터리를 검색하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  find
  </blockquote>
  </details>

---

### 🛠️ 9. 실습형 문제
* **문제71** : 최상위 디렉터리 아래에 `/project` 디렉터리를 생성하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  mkdir /project
  </blockquote>
  </details>

* **문제72** : `memo.txt` 파일을 생성한 후, 바로 파일의 내용을 확인하는 명령어를 차례대로 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  touch memo.txt<br>cat memo.txt
  </blockquote>
  </details>

* **문제73** : `test.txt` 파일의 권한을 755(rwxr-xr-x)로 변경하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo chmod 755 test.txt
  </blockquote>
  </details>

* **문제74** : 실행 중인 프로세스 중 `nginx` 프로세스만 필터링하여 검색하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  ps -ef | grep nginx
  </blockquote>
  </details>

* **문제75** : `backup/` 디렉터리를 `backup.tar.gz`라는 이름의 압축 파일로 만드는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  tar czvf backup.tar.gz backup/
  </blockquote>
  </details>

---

### ⚙️ 10. 운영형 문제
* **문제76** : Nginx 설정 파일 변경 후, 변경 사항을 적용하기 위해 가장 먼저 해야 하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo systemctl restart nginx (또는 sudo systemctl reload nginx)
  </blockquote>
  </details>

* **문제77** : 신입 사용자를 위한 `newUser` 계정을 생성하고, `sudo` 권한 그룹에 포함시키는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo adduser newUser<br>sudo usermod -aG sudo newUser
  </blockquote>
  </details>

* **문제78** : 서버 저장 공간(디스크)이 부족할 때, 전체적인 디스크 사용량을 확인하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  df -h
  </blockquote>
  </details>

* **문제79** : 서버 CPU 사용량이 급증했을 때, 어떤 프로세스가 원인인지 실시간으로 확인하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  top (또는 htop)
  </blockquote>
  </details>

* **문제80** : 서버가 재부팅되어도 특정 디스크가 자동으로 연결(마운트)되도록 설정하려면 어떤 파일을 수정해야 하나요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  /etc/fstab
  </blockquote>
  </details>

---

### 🚨 11. 장애 대응형
* **문제81** : 웹 사이트 접속이 안 될 때, Nginx 서비스의 구동 상태(에러 메시지 등)를 확인하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo systemctl status nginx
  </blockquote>
  </details>

* **문제82** : 특정 프로세스가 응답하지 않고 정상 종료되지 않을 때, 강제로 프로세스를 종료하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  kill -9 [PID]
  </blockquote>
  </details>

* **문제83** : 네트워크 장애 시, DNS 서버가 도메인 주소를 잘 해석하고 있는지 확인할 때 사용하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  nslookup google.com
  </blockquote>
  </details>

* **문제84** : 다른 서버나 외부 네트워크와의 연결 상태를 확인하는 가장 기본적인 네트워크 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  ping 8.8.8.8
  </blockquote>
  </details>

* **문제85** : 시스템 주요 로그 파일인 `syslog`를 실시간으로 모니터링하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  tail -f /var/log/syslog
  </blockquote>
  </details>

---

### 🌐 12. 서버 구축형
* **문제86** : Ubuntu 환경에서 Nginx 웹 서버를 설치하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo apt install -y nginx
  </blockquote>
  </details>

* **문제87** : 서버가 부팅될 때 Nginx 서비스가 자동으로 시작되도록 설정하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo systemctl enable nginx
  </blockquote>
  </details>

* **문제88** : 새로운 디스크 파티션 `/dev/sdb1`을 `/data` 디렉터리에 마운트하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo mount /dev/sdb1 /data
  </blockquote>
  </details>

* **문제89** : 새로운 사용자 계정을 생성하는 기본 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo adduser [사용자명]
  </blockquote>
  </details>

* **문제90** : 패키지 매니저에서 최신 패키지 목록 정보를 동기화(최신화)하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo apt update
  </blockquote>
  </details>

---

### 🪵 13. 로그 분석형
* **문제91** : Nginx 서비스의 로그 기록만 지정해서 확인하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  journalctl -u nginx
  </blockquote>
  </details>

* **문제92** : 특정 로그 파일(`filename.log`)의 맨 마지막 50줄만 확인하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  tail -50 filename.log
  </blockquote>
  </details>

* **문제93** : 로그 파일(`logfile.log`) 내에서 대소문자 구분 없이 `error`라는 문자열만 포함된 라인을 검색하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  grep error logfile.log
  </blockquote>
  </details>

* **문제94** : 로그 파일의 갱신 상태를 실시간으로 화면에 출력하며 모니터링하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  tail -f logfile.log
  </blockquote>
  </details>

* **문제95** : 시스템 전체의 로그를 확인할 때 사용하는 핵심 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  journalctl
  </blockquote>
  </details>
---

### 🛡️ 14. 보안형
* **문제96** : 특정 파일의 권한을 파일 소유자만 읽고 쓸 수 있도록 제한하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo chmod 600 filename
  </blockquote>
  </details>

* **문제97** : 일반 사용자 계정에서 root(관리자) 권한으로 명령을 실행할 때 앞에 붙이는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  sudo
  </blockquote>
  </details>

* **문제98** : 현재 시스템에서 `sudo` 권한을 가진 그룹의 정보를 확인하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  getent group sudo
  </blockquote>
  </details>

* **문제99** : 리눅스에서 사용자의 암호화된 비밀번호가 안전하게 저장되는 파일의 경로는 어디인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  /etc/shadow
  </blockquote>
  </details>

* **문제100** : 실무에서 `chmod 777` 명령어 사용을 강력히 지양하는 이유는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  시스템 내부의 모든 사용자에게 읽기, 쓰기, 실행 권한이 전부 개방되어 보안상 매우 치명적인 위험을 초래할 수 있기 때문입니다.
  </blockquote>
  </details>

---

### 💾 15. 스토리지형
* **문제101** : 시스템에 연결된 전체 디스크의 구조와 파티션 연결 상태를 트리 형태로 확인하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  lsblk
  </blockquote>
  </details>

* **문제102** : 특정 파티션에 `ext4` 포맷으로 파일 시스템을 생성하는 명령어를 작성하세요.
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  mkfs.ext4 [디바이스명] (예: mkfs.ext4 /dev/sdb1)
  </blockquote>
  </details>

* **문제103** : 마운트된 디스크들의 전체 크기, 사용량, 남은 공간을 사람이 보기 편한 단위(GB, MB 등)로 확인하는 명령어는 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  df -h
  </blockquote>
  </details>

* **문제104** : RAID 1(미러링) 구성 방식의 핵심적인 특징과 장점은 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  두 개 이상의 디스크에 데이터를 동시에 동일하게 복제하여 저장하는 미러링 방식입니다. 하나의 디스크가 고장 나더라도 데이터가 유실되지 않아 데이터 안정성이 매우 높습니다.
  </blockquote>
  </details>

* **문제105** : LVM(Logical Volume Manager)을 도입했을 때 실무 환경에서 얻을 수 있는 가장 큰 장점은 무엇인가요?
  <details>
  <summary>정답 확인 (클릭)</summary>
  <blockquote>
  운영 중인 서비스를 중단하거나 디스크를 분리하지 않고도, 온라인 상태에서 디스크 용량을 유연하게 확장할 수 있다는 점입니다.
  </blockquote>
  </details>





  
