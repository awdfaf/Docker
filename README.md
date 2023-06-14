# Docker 기초 공부

## 0. 예비 실습

[도커와 마이크로서비스 이해1 ](https://www.notion.so/1-301bfb1aaafe4d81bcfdfc8e809dcf96?pvs=21)

[도커와 마이크로서비스 이해2 ](https://www.notion.so/2-6f9ae8bda39447a38e621bf4a9f3278f?pvs=21)

[도커 컨테이너 활용법 이론 ](https://www.notion.so/58f0095963d744099b7154466aa3da40?pvs=21)

[도커 컨테이너 환경 구축 ](https://www.notion.so/18cabc0e5a7c476bb0795f146d5e9488?pvs=21)

[도커 컨테이너 실행 및 정보 확인 ](https://www.notion.so/0302a8371e9c4abdb5daf246add3f698?pvs=21)

[도커 컨테이너 여러개 동작 내부쉘 ](https://www.notion.so/dbabcffb8bab4dc3ac1b43d3639e542d?pvs=21)

[도커 컨테이너 웹 페이지 수정 방법 ](https://www.notion.so/993b3edf49554dcbaa82096ed4b00b76?pvs=21)

[도커 이미지 변경 후 허브에 업로드 ](https://www.notion.so/9795ab6bfb90440ab79767dbf0f63e6f?pvs=21)

[도커 볼륨 생성 및 활용 ](https://www.notion.so/e5916caec4b64723bd914a6649acfae8?pvs=21)

[도커 볼륨을 이용한 데이터베이스 운영 ](https://www.notion.so/c5a58699bfca452bbbc1fc1a508504e3?pvs=21)

[도커 네트워크 생성 및 활용 ](https://www.notion.so/4f06a777b4e04451a3140828b8eb51c7?pvs=21)

[동작중인 서버 모를때 ](https://www.notion.so/e3cde728eea54dd29d1d365990218d80?pvs=21)

[도커 볼륨을 활용한 웹페이지 변경 ](https://www.notion.so/098e09662d134c739ae1ea5e9432d9ec?pvs=21)

[도커 로드밸런싱 구축하기 ](https://www.notion.so/ea5b2bc8f4ba4b069db2ae8c9d8cba07?pvs=21)

[도커 파일 활용 이론 ](https://www.notion.so/1f8ac8508045480ca7341186e8df21af?pvs=21)

[도커 파일 활용하기 ](https://www.notion.so/69135f0b44e64528ba9a7ef6c9161903?pvs=21)

[도커 파일로 웹서버와 빌더 구축 ](https://www.notion.so/1defbfa6efbc43cc9202d39295026f2b?pvs=21)

[도커 파일 모범 활용 사례 ](https://www.notion.so/053b4f06a647424694e48092ea4f9ae1?pvs=21)

[도커 파일 불필요한 이미지 ](https://www.notion.so/dd5033843a1b4f14bb4dfdf1fb97886d?pvs=21)

[도커 컴포즈로 워드프레스 환경 구축 ](https://www.notion.so/02047d1055224336b97855f3f6ccf8a5?pvs=21)

[도커 로그 살펴보기 ](https://www.notion.so/84bc663a878e48549748b21dde762d2f?pvs=21)

---

## 1. 컨테이너와 도커의 이해

[[따배도] 1. 컨테이너와 도커의 이해 - 컨테이너를 쓰는이유 / 일반프로그램과 컨테이너프로그램의 차이점](https://www.youtube.com/watch?v=3HId-tpYaZs&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=2&ab_channel=TTABAE-LEARN)

### 컨테이너를 배우는 이유

### 이 시대가 원한다.

![Untitled](images/Untitled.png)

소프트웨어 운영 플랫폼이 바뀌고 있다.

![Untitled](images/Untitled%201.png)

### 왜 리눅스에서 실행할까?

<aside>
💡 리눅스 커널 기능을 써야하니까

</aside>

- chroot - 독립된 공간 형성
- namespace - isolate 기능 지원
- cgroup - 필요한만큼 HW지원

![Untitled](images/Untitled%202.png)

![Untitled](images/Untitled%203.png)

### 일반프로그램과의 차이점

- 하는 일은 같다. 생긴 모양이 다른것

![Untitled](images/Untitled%204.png)

### 도커를 사용하는 이유

<aside>
💡 개발자가 만든 그대로 어디서든 돌아간다. 
확장/축소 쉽고 MSA, DevOps에 적합하다.

</aside>

![Untitled](images/Untitled%205.png)

![Untitled](images/Untitled%206.png)

## 2. 도커 설치하기

[[따배도] 2. 도커 설치하기 - 학습편(준비물/실습 유형 소개)](https://www.youtube.com/watch?v=6S4CXKt6ibE&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=3&ab_channel=TTABAE-LEARN)

[[따배도] 2-1. 도커 설치하기:  Virtualbox 설치 / VM 생성](https://www.youtube.com/watch?v=PqgWp7rbqws&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=4&ab_channel=TTABAE-LEARN)

[[따배도] 2-2. 도커 설치하기: 우분투(Ubuntu) 설치](https://www.youtube.com/watch?v=REYVRyXdSKU&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=6&ab_channel=TTABAE-LEARN)

[[따배도] 2-3. 도커 설치하기: CentOS 설치 및 네트워크 구성](https://www.youtube.com/watch?v=xNby1hi3dow&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=7&ab_channel=TTABAE-LEARN)

### 도커 설치 준비

![Untitled](images/Untitled%207.png)

1. virturalbox(Hypervisor) 설치 - 네트워크 구성 - VM만들기
2. VM에 Ubuntu 설치하고 기본환경 구성
3. VM에 Centos 설치하고 기본환경 구성
4. Ubuntu/Centos Server에 Docker 설치
5. Windows에 DokcerDesktop 설치

### Virtualbox 설치

![Untitled](images/Untitled%208.png)

![Untitled](images/Untitled%209.png)

[Oracle VM VirtualBox](https://www.virtualbox.org/)

![Untitled](images/Untitled%2010.png)

### 네트워크 구성

- Network Manager
    
    ![Untitled](images/Untitled%2011.png)
    
- NAT Networks
    
    ![Untitled](images/Untitled%2012.png)
    
    ![Untitled](images/Untitled%2013.png)
    
    ![Untitled](images/Untitled%2014.png)
    
    설정
    

### 가상머신 생성

- 새로만들기 : Linux Ubuntu
    
    ![Untitled](images/Untitled%2015.png)
    
    ![Untitled](images/Untitled%2016.png)
    
    ![Untitled](images/Untitled%2017.png)
    
    ![Untitled](images/Untitled%2018.png)
    
    ![Untitled](images/Untitled%2019.png)
    
- 설정
    
    ![Untitled](images/Untitled%2020.png)
    
    ![Untitled](images/Untitled%2021.png)
    
    ![Untitled](images/Untitled%2022.png)
    
- Centos 만들기(위랑 똑같이)
    
    ![Untitled](images/Untitled%2023.png)
    

### Ubuntu 설치

- 이미지 다운
    
    ![Untitled](images/Untitled%2024.png)
    
    [Enterprise Open Source and Linux | Ubuntu](https://ubuntu.com/)
    
    ![Untitled](images/Untitled%2025.png)
    
- 추가 설정 및 이미지 추가
    
    ![Untitled](images/Untitled%2026.png)
    
    ![Untitled](images/Untitled%2027.png)
    
    ![Untitled](images/Untitled%2028.png)
    
- 시작 버튼 클릭 - 설정
    
    ![Untitled](images/Untitled%2029.png)
    
    ![Untitled](images/Untitled%2030.png)
    
    ![Untitled](images/Untitled%2031.png)
    
    [VirtualBox 우분투 설치시 버튼 안보일때](https://www.bearpooh.com/101)
    
    ![Untitled](images/Untitled%2032.png)
    
    ![Untitled](images/Untitled%2033.png)
    
    ![Untitled](images/Untitled%2034.png)
    
    ![Untitled](images/Untitled%2035.png)
    
- 우분투 환경구성
    
    ![Untitled](images/Untitled%2036.png)
    
    ![Untitled](images/Untitled%2037.png)
    
- 터미널로 네트워크 구성
    
    ![Untitled](images/Untitled%2038.png)
    
    ![Untitled](images/Untitled%2039.png)
    
    [리눅스 키보드 오류 해결방법(입력모드 i)](https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=dlwjddns5&logNo=220656288619)
    
    ![Untitled](images/Untitled%2040.png)
    
    ![Untitled](images/Untitled%2041.png)
    
    ![Untitled](images/Untitled%2042.png)
    
- 네트워크 테스트
    
    ![Untitled](images/Untitled%2043.png)
    
- root 패스워드 설정
    
    ![Untitled](images/Untitled%2044.png)
    
    password
    
- 계정전환
    
    ![Untitled](images/Untitled%2045.png)
    
- 부팅방식 변경-TEXT모드
    
    ![Untitled](images/Untitled%2046.png)
    
- SSH 설치
    
    ![Untitled](images/Untitled%2047.png)
    
    ![Untitled](images/Untitled%2048.png)
    
    ![Untitled](images/Untitled%2049.png)
    
    ![Untitled](images/Untitled%2050.png)
    
    ![Untitled](images/Untitled%2051.png)
    
- Xshell
    
    [XSHELL - NetSarang Website](https://www.netsarang.com/ko/xshell/)
    
    ![Untitled](images/Untitled%2052.png)
    
    ![Untitled](images/Untitled%2053.png)
    
    포트포워딩 확인
    
    ![Untitled](images/Untitled%2054.png)
    
- 접속
    
    ![Untitled](images/Untitled%2055.png)
    
    ![Untitled](images/Untitled%2056.png)
    
    ![Untitled](images/Untitled%2057.png)
    
- 스냅샷
    
    ![Untitled](images/Untitled%2058.png)
    
    메모리 줄이기
    
    ![Untitled](images/Untitled%2059.png)
    
    ![Untitled](images/Untitled%2060.png)
    

### Centos 설치

[The CentOS Project](https://www.centos.org/)

영상보고 따라하기

### OS에 Docker 설치

![Untitled](images/Untitled%2061.png)

- 준비
    
    ![Untitled](images/Untitled%2062.png)
    
- 설치
    
    [Docker Docs: How to build, share, and run applications](https://docs.docker.com/)
    
    ![Untitled](images/Untitled%2063.png)
    
    ![Untitled](images/Untitled%2064.png)
    
- 확인
    
    ![Untitled](images/Untitled%2065.png)
    
- 도커 관리자 권한 부여
    
    ![Untitled](images/Untitled%2066.png)
    
    도커는 시스템 관리자인 root만 사용가능
    
    ![Untitled](images/Untitled%2067.png)
    
    관리자 권한 부여 완료
    

## 3-1. 도커 컨테이너 - 이론

[[따배도] 3-1. 도커 컨테이너 살펴보기: 이론편](https://www.youtube.com/watch?v=m454YTyPWSk&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=10&ab_channel=TTABAE-LEARN)

### 컨테이너와 컨테이너 이미지

![Untitled](images/Untitled%2068.png)

![Untitled](images/Untitled%2069.png)

![Untitled](images/Untitled%2070.png)

### 컨테이너 동작방식

![Untitled](images/Untitled%2071.png)

![Untitled](images/Untitled%2072.png)

![Untitled](images/Untitled%2073.png)

## 3-2. 도커 컨테이너 - 실습

[[따배도] 3-2. 도커 컨테이너 살펴보기: 실습편](https://www.youtube.com/watch?v=gNsjVOuF2jY&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=10&ab_channel=TTABAE-LEARN)

### DockerHub에서 이미지 검색

- 준비
    
    ![Untitled](images/Untitled%2074.png)
    
    ![Untitled](images/Untitled%2075.png)
    
    루트 전환
    
    ![Untitled](images/Untitled%2076.png)
    
    세션복제로 하나 더 생성
    
    ![Untitled](images/Untitled%2077.png)
    
    버전 확인
    
- 도커 동작 확인
    
    ![Untitled](images/Untitled%2078.png)
    
- 이미지 검색
    
    ![Untitled](images/Untitled%2079.png)
    

### image 다운로드 후 image layer 보기

![Untitled](images/Untitled%2080.png)

- 레이어 확인
    
    ![Untitled](images/Untitled%2081.png)
    
    ![Untitled](images/Untitled%2082.png)
    
    이미지 없음
    
- 이미지 다운
    
    ![Untitled](images/Untitled%2083.png)
    
    ![Untitled](images/Untitled%2084.png)
    
    레이어 이미지 5개 다운
    

### 컨테이너 실행 후 확인

- 이미지 확인
    
    ![Untitled](images/Untitled%2085.png)
    
- 컨테이너 실행
    
    ![Untitled](images/Untitled%2086.png)
    
- 확인
    
    ![Untitled](images/Untitled%2087.png)
    
- 중지
    
    ![Untitled](images/Untitled%2088.png)
    
- 컨테이너 삭제
    
    ![Untitled](images/Untitled%2089.png)
    
- 이미지 삭제
    
    ![Untitled](images/Untitled%2090.png)
    

## 4-1. 도커 컨테이너 만들어보기 - 이론

[[따배도] 4-1. 도커 컨테이너 만들어보기: 이론편](https://www.youtube.com/watch?v=9qnD8aODu-4&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=12&ab_channel=TTABAE-LEARN)

### 무엇을 컨테이너로 만드는가?

![Untitled](images/Untitled%2091.png)

![Untitled](images/Untitled%2092.png)

### 어떻게 컨테이너를 만드는가?

![Untitled](images/Untitled%2093.png)

![Untitled](images/Untitled%2094.png)

![Untitled](images/Untitled%2095.png)

![Untitled](images/Untitled%2096.png)

### 컨테이너를 배포하려면?

![Untitled](images/Untitled%2097.png)

## 4-2. 도커 컨테이너 만들어보기 - 실습

[[따배도] 4-2. 도커 컨테이너 만들어보기: 실습](https://www.youtube.com/watch?v=WLjfzwdASbw&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=13&ab_channel=TTABAE-LEARN)

### 실습 환경 확인 및 Node.js 소스코드 작성

![Untitled](images/Untitled%2098.png)

![Untitled](images/Untitled%2099.png)

### Docker File 작성

![Untitled](images/Untitled%20100.png)

![Untitled](images/Untitled%20101.png)

### 컨테이너 이미지 빌드

![Untitled](images/Untitled%20102.png)

![Untitled](images/Untitled%20103.png)

### 우분투 웹 서버 컨테이너 이미지 만들고 빌드

![Untitled](images/Untitled%20104.png)

![Untitled](images/Untitled%20105.png)

![Untitled](images/Untitled%20106.png)

![Untitled](images/Untitled%20107.png)

- 확인
    
    ![Untitled](images/Untitled%20108.png)
    

### 만들어놓은 컨테이너 배포하기

- 로그인 → 태그 설정 → 배포
    
    ![Untitled](images/Untitled%20109.png)
    
    ![Untitled](images/Untitled%20110.png)
    
    ![Untitled](images/Untitled%20111.png)
    

## 5-1. 컨테이너 보관창고 - 이론

[[따배도] 5-1. 컨테이너 보관창고 - 이론편](https://www.youtube.com/watch?v=aFIj68YuvzQ&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=15&ab_channel=TTABAE-LEARN)

![Untitled](images/Untitled%20112.png)

### Registry

![Untitled](images/Untitled%20113.png)

### Docker hub 사용해보기

![Untitled](images/Untitled%20114.png)

![Untitled](images/Untitled%20115.png)

### Private Registry 구축

![Untitled](images/Untitled%20116.png)

![Untitled](images/Untitled%20117.png)

## 5-2. 컨테이너 보관창고 - 실습

[[따배도] 5-2. 컨테이너 보관창고(Docker Registry) - 실습](https://www.youtube.com/watch?v=bQ6XxI0Ep_Q&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=14&ab_channel=TTABAE-LEARN)

### Public Registry(Docker hub)

- 이미지 검색
    
    ![Untitled](images/Untitled%20118.png)
    
- 이미지 다운
    
    ![Untitled](images/Untitled%20119.png)
    
- 도커 허브 레파지토리에 업로드
    
    ![Untitled](images/Untitled%20120.png)
    
    ![Untitled](images/Untitled%20121.png)
    

### Public Registry 운영하기

![Untitled](images/Untitled%20122.png)

![Untitled](images/Untitled%20123.png)

- 레지스트리 컨테이너 실행
    
    ![Untitled](images/Untitled%20124.png)
    
- 로컬 저장소에 업로드
    
    ![Untitled](images/Untitled%20125.png)
    
- 확인
    
    ![Untitled](images/Untitled%20126.png)
    

## 6-1. Docker 컨테이너 사용 - 이론

[[따배도] 6-1. Docker 컨테이너 사용하기 - 이론편](https://www.youtube.com/watch?v=ild9PzdC0ww&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=15&ab_channel=TTABAE-LEARN)

### 컨테이너 이미지 사용

![Untitled](images/Untitled%20127.png)

![Untitled](images/Untitled%20128.png)

### 컨테이너 실행 라이프 사이클

![Untitled](images/Untitled%20129.png)

![Untitled](images/Untitled%20130.png)

![Untitled](images/Untitled%20131.png)

### 동작중인 컨테이너 관리

![Untitled](images/Untitled%20132.png)

![Untitled](images/Untitled%20133.png)

## 6-2. Docker 컨테이너 사용 -실습

[[따배도] 6-2. Docker 컨테이너 사용하기 - 실습편](https://www.youtube.com/watch?v=wrx-ixvtzxk&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=16&ab_channel=TTABAE-LEARN)

→ 이미 보안 공부할 때 다해봤던것. 생략

![Untitled](images/Untitled%20134.png)

![Untitled](images/Untitled%20135.png)

![Untitled](images/Untitled%20136.png)

![Untitled](images/Untitled%20137.png)

![Untitled](images/Untitled%20138.png)

![Untitled](images/Untitled%20139.png)

![Untitled](images/Untitled%20140.png)

![Untitled](images/Untitled%20141.png)

![Untitled](images/Untitled%20142.png)

![Untitled](images/Untitled%20143.png)

![Untitled](images/Untitled%20144.png)

![Untitled](images/Untitled%20145.png)

![Untitled](images/Untitled%20146.png)

![Untitled](images/Untitled%20147.png)

![Untitled](images/Untitled%20148.png)

![Untitled](images/Untitled%20149.png)

![Untitled](images/Untitled%20150.png)

![Untitled](images/Untitled%20151.png)

![Untitled](images/Untitled%20152.png)

## 7-1. Docker 컨테이너 리소스 관리 - 이론

[[따배도] 7-1. Docker 컨테이너 리소스를 관리해야지 - 이론편](https://www.youtube.com/watch?v=7HA_00KNtbc&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=17&ab_channel=TTABAE-LEARN)

### 컨테이너 리소스 제한

![Untitled](images/Untitled%20153.png)

![Untitled](images/Untitled%20154.png)

### Memory 리소스 제한

![Untitled](images/Untitled%20155.png)

### CPU 리소스 제한

![Untitled](images/Untitled%20156.png)

### Block I/O 제한

![Untitled](images/Untitled%20157.png)

### 리소스 모니터링

![Untitled](images/Untitled%20158.png)

## 7-2. Docker 컨테이너 리소스 관리 - 실습

[[따배도] 7-2. Docker 컨테이너 리소스를 관리해야지 - 실습편](https://www.youtube.com/watch?v=TM3DvwwvsLg&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=18&ab_channel=TTABAE-LEARN)

### 부하 테스트 프로그램 - Stress

![Untitled](images/Untitled%20159.png)

![Untitled](images/Untitled%20160.png)

![Untitled](images/Untitled%20161.png)

![Untitled](images/Untitled%20162.png)

### Memory 리소스 제한 실습

![Untitled](images/Untitled%20163.png)

![Untitled](images/Untitled%20164.png)

![Untitled](images/Untitled%20165.png)

### CPU 리소스 제한 실습

![Untitled](images/Untitled%20166.png)

![Untitled](images/Untitled%20167.png)

![Untitled](images/Untitled%20168.png)

![Untitled](images/Untitled%20169.png)

![Untitled](images/Untitled%20170.png)

![Untitled](images/Untitled%20171.png)

![Untitled](images/Untitled%20172.png)

![Untitled](images/Untitled%20173.png)

![Untitled](images/Untitled%20174.png)

### Block I/O 제한 실습

![Untitled](images/Untitled%20175.png)

![Untitled](images/Untitled%20176.png)

### cAdvisor 실행

![Untitled](images/Untitled%20177.png)

![Untitled](images/Untitled%20178.png)

![Untitled](images/Untitled%20179.png)

## 8-1. Docker Container Storage - 이론

[[따배도] 8-1. Docker Container Storage - 이론편](https://www.youtube.com/watch?v=JcgrQnkIePE&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=19&ab_channel=TTABAE-LEARN)

### 컨테이너 볼륨

![Untitled](images/Untitled%20180.png)

![Untitled](images/Untitled%20181.png)

![Untitled](images/Untitled%20182.png)

![Untitled](images/Untitled%20183.png)

### 컨테이너끼리 데이터 공유

![Untitled](images/Untitled%20184.png)

## 8-2. Docker Container Storage - 실습

[[따배도] 8-2. Docker Container Storage - 실습편](https://www.youtube.com/watch?v=IHuU3rZATbg&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=20&ab_channel=TTABAE-LEARN)

### Mysql DB data 영구 보존하기

![Untitled](images/Untitled%20185.png)

![Untitled](images/Untitled%20186.png)

![Untitled](images/Untitled%20187.png)

![Untitled](images/Untitled%20188.png)

![Untitled](images/Untitled%20189.png)

---

![Untitled](images/Untitled%20190.png)

![Untitled](images/Untitled%20191.png)

![Untitled](images/Untitled%20192.png)

![Untitled](images/Untitled%20193.png)

![Untitled](images/Untitled%20194.png)

### 웹데이터를 컨테이너에 지원하기

![Untitled](images/Untitled%20195.png)

![Untitled](images/Untitled%20196.png)

이후 html 수정해도 바로 반영

### 컨테이너끼리 데이터 공유

![Untitled](images/Untitled%20197.png)

![Untitled](images/Untitled%20198.png)

![Untitled](images/Untitled%20199.png)

![Untitled](images/Untitled%20200.png)

![Untitled](images/Untitled%20201.png)

![Untitled](images/Untitled%20202.png)

![Untitled](images/Untitled%20203.png)

![Untitled](images/Untitled%20204.png)

## 9-1. 컨테이너간 통신(네트워크) - 이론

[[따배도] 9-1. 컨테이너간 통신(네트워크) - 이론편](https://www.youtube.com/watch?v=jOX80bXND2w&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=21&ab_channel=TTABAE-LEARN)

### 컨테이너는 어떻게 통신하나?

![Untitled](images/Untitled%20205.png)

### 컨테이너 포트를 외부로 노출할 수 있나?

![Untitled](images/Untitled%20206.png)

### 컨테이너 네트워크를 추가할 수 있나?

![Untitled](images/Untitled%20207.png)

### 컨테이너끼리 통신은?

![Untitled](images/Untitled%20208.png)

## 9-2. 컨테이너간 통신(네트워크) - 실습

[[따배도] 9-2. 컨테이너간 통신(네트워크) - 실습편](https://www.youtube.com/watch?v=CXrrkl4Zamc&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=22&ab_channel=TTABAE-LEARN)

### 컨테이너 네트워크 사용하기

![Untitled](images/Untitled%20209.png)

![Untitled](images/Untitled%20210.png)

![Untitled](images/Untitled%20211.png)

![Untitled](images/Untitled%20212.png)

![Untitled](images/Untitled%20213.png)

![Untitled](images/Untitled%20214.png)

### 컨테이너 포트 외부로 노출하기

![Untitled](images/Untitled%20215.png)

![Untitled](images/Untitled%20216.png)

![Untitled](images/Untitled%20217.png)

![Untitled](images/Untitled%20218.png)

### user-defined network 구성

![Untitled](images/Untitled%20219.png)

![Untitled](images/Untitled%20220.png)

![Untitled](images/Untitled%20221.png)

![Untitled](images/Untitled%20222.png)

![Untitled](images/Untitled%20223.png)

![Untitled](images/Untitled%20224.png)

### 컨테이너 서비스 운영

![Untitled](images/Untitled%20225.png)

![Untitled](images/Untitled%20226.png)

![Untitled](images/Untitled%20227.png)

## 10-1. 빌드에서 운영까지(Using Docker Compose) - 이론

[[따배도] 10-1. 빌드에서 운영까지 (using Docker Compose) - 이론편](https://www.youtube.com/watch?v=AYRVKB1L0Ak&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=23&ab_channel=TTABAE-LEARN)

### 도커 컴포즈?

![Untitled](images/Untitled%20228.png)

### 도커 컴포즈로 컨테이너 실행이 가능한가?

![Untitled](images/Untitled%20229.png)

![Untitled](images/Untitled%20230.png)

![Untitled](images/Untitled%20231.png)

![Untitled](images/Untitled%20232.png)

### 빌드에서 운영까지

![Untitled](images/Untitled%20233.png)

## 10-2. 빌드에서 운영까지(Using Docker Compose) - 실습

[[따배도] 10-2. 빌드에서 운영까지 (using Docker Compose) - 실습편](https://www.youtube.com/watch?v=f8yLLWaXtCM&list=PLApuRlvrZKogb78kKq1wRvrjg1VMwYrvi&index=24&ab_channel=TTABAE-LEARN)

### 도커 컴포즈 설치하기

[Try Docker Compose](https://docs.docker.com/compose/gettingstarted/)

![Untitled](images/Untitled%20234.png)

![Untitled](images/Untitled%20235.png)

![Untitled](images/Untitled%20236.png)

### 컨테이너 빌드에서 운영까지

![Untitled](images/Untitled%20237.png)

![Untitled](images/Untitled%20238.png)

![Untitled](images/Untitled%20239.png)

![Untitled](images/Untitled%20240.png)

![Untitled](images/Untitled%20241.png)

![Untitled](images/Untitled%20242.png)

![Untitled](images/Untitled%20243.png)

![Untitled](images/Untitled%20244.png)

![Untitled](images/Untitled%20245.png)

![Untitled](images/Untitled%20246.png)

![Untitled](images/Untitled%20247.png)

![Untitled](images/Untitled%20248.png)

![Untitled](images/Untitled%20249.png)

![Untitled](images/Untitled%20250.png)

![Untitled](images/Untitled%20251.png)

![Untitled](images/Untitled%20252.png)

![Untitled](images/Untitled%20253.png)

![Untitled](images/Untitled%20254.png)

![Untitled](images/Untitled%20255.png)

![Untitled](images/Untitled%20256.png)

### MySQL 사용하는 WordPress 운영

[awesome-compose/README.md at master · docker/awesome-compose](https://github.com/docker/awesome-compose/blob/master/official-documentation-samples/wordpress/README.md)

![Untitled](images/Untitled%20257.png)

![Untitled](images/Untitled%20258.png)

![Untitled](images/Untitled%20259.png)

![Untitled](images/Untitled%20260.png)
