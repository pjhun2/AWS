# AWS
AWS EC2 사용방법

https://aws.amazon.com/ko/

AWS 계정 생성

콘솔에 로그인 이후 EC2 선택
![image](https://user-images.githubusercontent.com/74689088/106374384-5f641100-63c6-11eb-8da2-c7bb503b1adb.png)


인스턴스에서 사용 중인 인스턴스와 새로운 인스턴스 생성 가능
![image](https://user-images.githubusercontent.com/74689088/106374421-c7b2f280-63c6-11eb-9c0a-cf1dd2278bcc.png)

인스턴스 시작으로 새로운 인스턴스 생성
![image](https://user-images.githubusercontent.com/74689088/106374443-f92bbe00-63c6-11eb-916e-6b93fa94055a.png)



생성할 인스턴스의 OS 선택 ( Windows , Linux , Mac OS ) 
![image](https://user-images.githubusercontent.com/74689088/106374459-09439d80-63c7-11eb-9ad5-86b3807a68d0.png)

OS 확인 후 아래 선택 버튼으로 생성 진행
![image](https://user-images.githubusercontent.com/74689088/106374485-28dac600-63c7-11eb-9b54-c289292af495.png)

EC2 무료 제공 cpu와 메모리 확인 후 검토 및 시작
![image](https://user-images.githubusercontent.com/74689088/106374501-4ad44880-63c7-11eb-9153-182eac4af175.png)

기본적으로 0.0.0.0으로 모든 대역 허용  
설정을 변경하려면  
6. 보안 그룹 구성 -> 소스 -> 드롭박스에서 내 IP로 지정
![image](https://user-images.githubusercontent.com/74689088/106374531-75260600-63c7-11eb-8c4f-a5225da0f0e4.png)

설정 완료 후 시작하기로 인스턴스 시작
![image](https://user-images.githubusercontent.com/74689088/106374600-22991980-63c8-11eb-903d-ec1ac0c028cf.png)

처음 생성 시에 새 키 페어를 생성하여 인스턴스에 연결해야함  
이름을 지정한 후 키 페어를 다운로드 후 인스턴스 시작
![image](https://user-images.githubusercontent.com/74689088/106374616-3c3a6100-63c8-11eb-87d1-c0429082828a.png)

원격에서 접속하기 위해 생성한 인스턴스에 IP 할당
![image](https://user-images.githubusercontent.com/74689088/106374918-b370f480-63ca-11eb-92ce-011d486f354c.png)  
![image](https://user-images.githubusercontent.com/74689088/106374937-f763f980-63ca-11eb-9552-d8f064bbdd20.png)

할당된 IPV4 주소 클릭
![image](https://user-images.githubusercontent.com/74689088/106374968-4578fd00-63cb-11eb-937f-dea4b8368ff8.png)  

탄력적 IP 주소 연결
![image](https://user-images.githubusercontent.com/74689088/106374983-5cb7ea80-63cb-11eb-8bfc-d187193b3d9e.png)

인스턴스 선택 후 연결
![image](https://user-images.githubusercontent.com/74689088/106375004-8f61e300-63cb-11eb-9122-0563e2fe44d7.png)

인스턴스 접속 SSH  
Windows의 경우 puttygen을 사용하여 개인키를 생성하여 접속
![image](https://user-images.githubusercontent.com/74689088/106375020-c932e980-63cb-11eb-9562-7687c9a7951f.png)

Load로 이전에 다운로드받은 Pem파일 로드  
로드 후 Save Private key로 개인키를 로컬에 저장
![image](https://user-images.githubusercontent.com/74689088/106375038-ebc50280-63cb-11eb-8380-0eaf4bee29a6.png)

Putty 접속 방법  
Host Name에 인스턴스에 할당한 IP 입력
![image](https://user-images.githubusercontent.com/74689088/106375049-11eaa280-63cc-11eb-8e41-ad64c846dc60.png)

왼쪽 옵션 SSH -> Auth -> private Key file for Authentication 에서 이전에 생성한 개인키 로드
![image](https://user-images.githubusercontent.com/74689088/106375069-44949b00-63cc-11eb-9808-90a324d8f10b.png)

Open하여 SSH 접속 로그인
ubuntu 입력 후 imported-openssh-key로 로그인
![image](https://user-images.githubusercontent.com/74689088/106375083-760d6680-63cc-11eb-96c0-4304c6bf71db.png)

이후 AWS Ubuntu 사용



