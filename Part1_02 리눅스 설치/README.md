## 02 리눅스 설치

### 설정
- 소프트웨어 선택 -> 서버 - GUI 사용 -> 개발용 도구
- 파티션 설정 -> 표준 파티션 -> + -> 마운트 지점 - (/boot, 1024)(swap, 2048)(/, *)
- password: lchy
- 목록에 없습니까? -> root -> password 설정한 거!

- 윈도우는 관리자, 사용자가 같은 곳에 위치
- 리눅스는 관리자, 사용자가 서로 다른 곳에 위치

### 리눅스 주요 디렉토리 관련 설명
- ls -l -> dictory의 목록들이 나온다.
- / 
    - 최상위 디렉토리 ==  리눅스상에 존재하는 모든 파일과 디렉토리의 시작. 최상위에 위치하는 디렉토리
- /boot 
    - 부팅 과정에 필요한 정보 파일들의 경로 == boot partition 설정시에는 1GB이상 용량을 설정

- /bin (binary)
    - 기본적인 명령어 실행파일들의 경로 == *.exe (실행파일)
- /sbin (system binary)
    - 시스템 운영, 관리에 필요한 명령어 경로 --> 관리자용 명령어 == *.exe (실행파일)
    - 일반 사용자들을 사용할 수 없다.

- /root
    - 디렉토리는 부팅할 때 이용하는 얘들 == 관리자(root)의 home directory
- /home
    -  일반 사용자들의 home directory가 저장되는 경로
    - home directory == 계정에 대한 정보를 저장하고 있는 디렉토리

- /dev
    - 각종 장치파일들이 저장되는 경로 == device
    - 리눅스 시스템은 장치를 장치로서 인식하는 것이 아니라 장치파일로 인식
- /etc (중요)
    - 서버 설정에 필요한 모든 정보파일들의 경로
- /usr
    - 윈도우 프로그램파일 폴더 유사 == 리눅스 응용프로그램 기본 설치 경로 == 대용량 데이타 보관 용도로도 사용
- /var 
    - 로그(log) 파일들의 경로
