# Linux_study

## 학습 
### Part1
  - 리눅스 개요 [NOTE01 📗] - 1강, 2강
  - 리눅스 설치 [NOTE02 📗] - 3강, 4강, 5강
  - 리눅스 네트워크 설정
  - 베이직 커맨드 (기본명령어)
  - 베이직 커맨드 (cp/mv)
  - vi editor
  - user account management
  - 권한(permission)
  - ownership
  - 특수권한(sticky bit / SetUID / SetGID)
  - ACL & 권한 응용 계정 관리
  - umask
  - compress1
  - compress2
  - RPM 1
  - filesystem & mount 
  - root password 관리 & GRUB bootloader
  - process
  - target mode(run level)


[NOTE01 📗]: https://github.com/chea-young/Linux_study/blob/main/Part1_01%20%EB%A6%AC%EB%88%85%EC%8A%A4%20%EA%B0%9C%EC%9A%94/README.md
[NOTE02 📗]:https://github.com/chea-young/Linux_study/tree/main/Part1_02%20%EB%A6%AC%EB%88%85%EC%8A%A4%20%EC%84%A4%EC%B9%98
### Part2  

### 추가적으로 배우개된 내용
- Linux에서 아파치 서버 실행
  - Apache Download
    - sudo apt-get install apache2
    - sudo service apache2 start: Apache 시작
      - sudo service apache2 stop: Apache 서버 멈추기
    - 'http://localhost'를 입력하면 웹서버 실행 완료
  - Apache setting
    - 시작 apache 서버 실행 위치는 '/var/www/html'
    - 초기 실행 위치를 수정하기
      - sudo nano /etc/apache2/apache2.conf
      - 수정: <Directory /var/www/html> -> <Directory [원하는 위치]>
      - sudo nano /etc/apache2/sites-enabled/000-default.conf
      - 수정: <Directory /var/www/html> -> <Directory [원하는 위치]>
      - sudo /etc/init.d/apache2 restart
