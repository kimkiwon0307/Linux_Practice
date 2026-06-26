<details>
<summary><h2>📋 리눅스 학습 문제 50선 (클릭하여 보기)</h2></summary>

1. **리눅스에서 커널의 역할은?**
   <details><summary>답보기</summary>하드웨어와 소프트웨어 사이를 연결하고 CPU, 메모리, 디스크, 네트워크 등의 자원을 관리한다.</details>

2. **절대경로와 상대경로의 차이를 설명하세요.**
   <details><summary>답보기</summary>절대경로는 / 부터 시작하고 상대 경로는 현재 위치부터 시작한다.</details>

3. **Soft Link와 Hard Link의 차이점은?**
   <details><summary>답보기</summary>하드 링크는 같은 inode를 공유하고 소프트링크는 원본 경로를 가리킨다.</details>

4. **systemctl 명령어의 역할은?**
   <details><summary>답보기</summary>서비스 시작, 중지, 재시작, 상태 확인, 자동 시작 설정 등을 관리한다.</details>

5. **SSH를 사용하는 이유는?**
   <details><summary>답보기</summary>원격 서버를 암호화된 통신으로 안전하게 관리하기 위해 사용한다.</details>

6. **RAID 1 특징은?**
   <details><summary>답보기</summary>미러링 방식으로 동일한 데이터를 두 디스크에 저장하여 장애 발생 시에도 데이터를 유지한다.</details>

7. **LVM을 사용하는 이유는?**
   <details><summary>답보기</summary>파티션을 유연하게 확장, 축소하고 여러 디스크를 하나처럼 관리하기 위해 사용한다.</details>

8. **Quota란?**
   <details><summary>답보기</summary>사용자 또는 그룹별 디스크 사용량을 제한하는 기능이다.</details>

9. **프로세스와 서비스의 차이는?**
   <details><summary>답보기</summary>프로세스는 실행중인 프로그램이고, 서비스는 백그라운드에서 지속적으로 동작하는 시스템 프로그램이다.</details>

10. **cron의 역할은?**
    <details><summary>답보기</summary>예약된 시간에 작업을 자동 실행한다.</details>

11. **현재 작업 디렉터리를 확인하는 명령어는?**
    <details><summary>답보기</summary>pwd</details>

12. **현재 위치의 파일 목록을 자세히 출력하는 명령어는?**
    <details><summary>답보기</summary>ls -al</details>

13. **새 사용자 생성 명령어는?**
    <details><summary>답보기</summary>sudo adduser user1</details>

14. **사용자 비밀번호 변경 명령어는?**
    <details><summary>답보기</summary>passwd user1</details>

15. **서비스 상태 확인 명령어는?**
    <details><summary>답보기</summary>sudo systemctl status 서비스명</details>

16. **실행 중인 프로세스를 확인하는 명령어는?**
    <details><summary>답보기</summary>ps -ef</details>

17. **프로세스를 강제 종료하는 명령어는?**
    <details><summary>답보기</summary>kill -9 PID</details>

18. **패키지 목록을 최신화 하는 명령어는?**
    <details><summary>답보기</summary>sudo apt update</details>

19. **Apache 설치 명령어는?**
    <details><summary>답보기</summary>sudo apt install -y apache2</details>

20. **SSH 서비스 재시작 명령어는?**
    <details><summary>답보기</summary>sudo systemctl restart sshd</details>

21. **student 사용자를 생성하시오.**
    <details><summary>답보기</summary>sudo adduser student</details>

22. **project 디렉터리를 생성하시오.**
    <details><summary>답보기</summary>sudo mkdir project</details>

23. **project 디렉터리 안에 test.txt 파일을 생성하시오.**
    <details><summary>답보기</summary>touch project/test.txt</details>

24. **test.txt 권한을 644로 변경하세요.**
    <details><summary>답보기</summary>sudo chmod 644 test.txt</details>

25. **student를 sudo 그룹에 추가하세요.**
    <details><summary>답보기</summary>sudo usermod -aG sudo student</details>

26. **새로운 Ubuntu 서버를 받았다. 가장 먼저 해야 할 작업 3가지는?**
    <details><summary>답보기</summary>1. 패키지업데이트 2.사용자 생성 및 sudo 권한 설정 3.SSH 설정 및 방화벽 설정</details>

27. **신입 사원이 입사했다. 어떤 리눅스 작업을 먼저 해야 하는가?**
    <details><summary>답보기</summary>사용자생성, 비밀번호 설정, 그룹 권한 부여, SSH 접근 설정</details>

28. **웹 서버를 구축할 때 기본 순서를 적으시오.**
    <details><summary>답보기</summary>1. 패키지 업데이트 2. Apache 설치 3. 서비스 실행 4. 방화벽 허용 5. 웹 페이지 배포 6.접속 확인</details>

29. **서비스가 자동 시작되지 않는다. 무엇을 확인해야하는가?**
    <details><summary>답보기</summary>systemctl is-enabled 서비스명</details>

30. **로그 확인 순서는?**
    <details><summary>답보기</summary>1.서비스 상태 확인 2.journalctl 확인 3.로그 파일 확인 4.설정 파일 확인</details>

31. **SSH 접속이 되지 않는다. 가장 먼저 확인할 것은?**
    <details><summary>답보기</summary>systemctl status ssh</details>

32. **웹 페이지가 열리지 않는다. 확인해야 할 항목 3가지는?**
    <details><summary>답보기</summary>서비스 실행 여부, 방화벽, 80포트 리스닝 여부</details>

33. **디스크가 가득 찼다. 어떤 명령어를 사용하는가?**
    <details><summary>답보기</summary>df -h</details>

34. **CPU 사용률이 매우 높다. 어떤 명령어를 사용하는가?**
    <details><summary>답보기</summary>top 또는 htop</details>

35. **실수로 서비스를 종료했다. 어떻게 복구하는가?**
    <details><summary>답보기</summary>sudo systemctl start 서비스명</details>

36. **Apache 설치 명령어는?**
    <details><summary>답보기</summary>sudo apt install -y apache2</details>

37. **Apache 자동 시작 설정 명령어는?**
    <details><summary>답보기</summary>sudo systemctl enable apache2</details>

38. **SSH 설치 명령어는?**
    <details><summary>답보기</summary>sudo apt install -y openssh-server</details>

39. **SSH 상태 확인 명령어는?**
    <details><summary>답보기</summary>sudo systemctl status ssh</details>

40. **SSH 포트를 확인하느 명령어는?**
    <details><summary>답보기</summary>sudo ss -tnlp | grep ssh</details>

41. **SSH 로그를 확인하는 명령어는?**
    <details><summary>답보기</summary>journalctl -u ssh</details>

42. **부팅 로그를 확인하는 명령어는?**
    <details><summary>답보기</summary>journalctl -b</details>

43. **실시간 로그를 확인하는 명령어는?**
    <details><summary>답보기</summary>tail -f /var/log/syslog</details>

44. **Apache 로그 위치는?**
    <details><summary>답보기</summary>/var/log/apache2/</details>

45. **최근 로그인 기록 확인 명령어는?**
    <details><summary>답보기</summary>last</details>

46. **root 계정으로 직접 SSH 로그인을 허용하지 않는 이유는?**
    <details><summary>답보기</summary>무자별 대입 공격 위험을 줄이고 보안을 강화하기 위해서이다.</details>

47. **파일 권한을 최소한으로 부여해야 하는 이유는?**
    <details><summary>답보기</summary>최소 권한 원칙을 적용해 불필요한 접근을 막기 위해서이다.</details>

48. **sudo를 사용하는 이유는?**
    <details><summary>답보기</summary>필요한 작업에만 관리자 권한을 부여하고, 작업 기록을 남겨 보안을 높이기 위해서이다.</details>

49. **SSH에서 비밀번호 인증 대신 공개키 인증을 사용하는 장점은?**
    <details><summary>답보기</summary>인증 보안 수준이 더 높다.</details>

50. **서버를 인터넷에 공개하기 전에 반드시 확인해야 할 보안 항목 3가지는?**
    <details><summary>답보기</summary>방화벽 설정, 최신 보안 업데이트 적용, 불필요한 서비스 비활성화</details>
</details>
