# netwhat

## 1) DHCP is used for ________
###   KEY) Both IPv6 and IPv4
* https://www.cisco.com/assets/sol/sb/RV320_Emulators/RV320_Emulator_v1-2-1-14/help/DHCP.html
* DHCP는 IPv4 and IPv6에 사용된다. 둘 다 지원을 한다.
* DHCP : 동적 호스트 구성 프로토콜 [udp]
* DHCP is used for IPv4 and IPv6. While both versions serve the same purpose, the details of the protocol for IPv4 and IPv6 are sufficiently different that they should be considered separate protocols.

## 2) Which of the following is private IP address?
###   KEY) 192.168.178.64
* 사설 ip주소를 고르는 문제이다.
* IP란? internet protocol. 인터넷에 연결되어 있는 각 장치들을 고유하게 식별할 수 있는 식별번호.
* ip주소에는 ipv4, ipv6 두 가지 버전이 있으며, 유동 아이피(DHCP) vs 고정 아이피 또는 공인 아이피 vs 사설 아이피로 나눌 수 있다.
* 사설 아이피의 대역: 10.0.0.0 – 10.255.255.255 / 172.16.0.0 – 172.31.255.255 / 192.168.0.0 – 192.168.255.255

## 3) Which of this is not a class of IP address?
###   KEY)  Class F
* IPv4는 네트워크를 더욱 효율적으로 분배하기 위해 네트워크를 클래스별로 나누는데, A,B,C,D,E 총 5개의 클래스로 나누어져 있다.
* https://velog.io/@hidaehyunlee/IP-address란#2-ip주소의-클래스abc-class란

## 4) Which of the following services use UDP? 1. DHCP 2. SMTP 3. FTP 4. HTTP
###   KEY)  1
* https://velog.io/@hidaehyunlee/%EB%8D%B0%EC%9D%B4%ED%84%B0%EA%B0%80-%EC%A0%84%EB%8B%AC%EB%90%98%EB%8A%94-%EC%9B%90%EB%A6%AC-OSI-7%EA%B3%84%EC%B8%B5-%EB%AA%A8%EB%8D%B8%EA%B3%BC-TCPIP-%EB%AA%A8%EB%8D%B8
* https://velog.io/@hidaehyunlee/TCP-%EC%99%80-UDP-%EC%9D%98-%EC%B0%A8%EC%9D%B4
* DHCP uses User Datagram Protocol (UDP), RFC 768, as its transport protocol. DHCP messages that a client sends to a server are sent to well-known port 67 (UDP Bootstrap Protocol and DHCP). DHCP Messages that a server sends to a client are sent to port 68.
* https://networkengineering.stackexchange.com/questions/64401/why-does-dhcp-use-udp-and-not-tcp
* DHCP: DHCP 서버를 사용하여 IP 주소 및 관련된 기타 구성 세부 정보를 네트워크의 DHCP 사용 클라이언트에게 동적으로 할당하는 방법을 제공한다.
* SMTP(Simple Mail Transfer Protocol): mail 전송 프로토콜. 데이터 전송의 신뢰성, 흐름 중요. TCP를 사용한다.
* FTP(File Transfer Protocol): 파일 전송 프로토콜. 데이터 전송의 신뢰성, 흐름 중요. TCP를 사용한다.
* HTTP(Hyper Text Transfer Protocol): 하이퍼텍스트 문서를 교환하기 위한 프로토콜. 인터넷에서 데이터를 주고받을 수 있는 프로토콜이다. 데이터 전송의 신뢰성, 흐름 중요. TCP를 사용한다.

## 5) Which of the following is the valid host range for the subnet on which the IP address 235.154.126.185/21 resides?
###   KEY)  235.154.120.1 ~ 235.154.127.254
* 11111111.11111111.11111000.00000000 & 235.154.126.185. 
* network address : 235.154.120.0(235.154.01111000.0)
* broadcast address : 235.154.127.255(235.154.011111111.1)

## 6) How long is an IPv6 address?
###   KEY)  128 bits
* IPv4 = 32bits

## 7) Which protocol does Ping use?
###   KEY)  ICMP
* ICMP : 인터넷 제어 메시지 프로토콜
* Ping이란? 네트워크 상태를 체크할 때 쓰이는 ICMP중 하나이다.
* ICMP란? ICMP는 TCP/IP에서 IP 패킷을 처리할 때 발생되는 문제를 알려주는 프로토콜이다.
* ICMP는 해당 호스트가 없거나, 해당 포트에 대기중에 서버 프로그램이 없는 등의 에러 상황이 발생할 경우 IP헤더에 기록되어 있는 출발지 호스트로 이러한 에러에 대한 상황을 보내주는 역할을 수행하게 된다.
* 그냥 정의 되어 있는 개념. 외워야 한다.
* BootP : 처음으로 부팅된 컴퓨터, 디스크를 갖지 않은 컴퓨터에게 IP 주소 등 구성정보를 제공, 정적인 클라이언트/서버 형태의 구성정보 제공용 프로토콜
* ARP : 주소 결정 프로토콜(Address Resolution Protocol, ARP)은 네트워크 상에서 IP 주소를 물리적 네트워크 주소로 대응(bind)시키기 위해 사용되는 프로토콜이다.
* https://biggerdata.tistory.com/41


## 8) You have an interface on a router with the IP address of 160.196.142.135/12. Including the router interface, how many hosts can have IP addresses on the LAN attached to the router interface?
###   KEY)  1048574
* 2^20 - 2

## 9) Which of this is not true?
###   KEY)  UDP doesn't supports Broadcasting
* 브로드캐스팅은 1:N 연결로 UDP가 지원한다.
* UDP는 비연결지향적. 속도를 중시한다.
* 체크섬(checksum)은 중복 검사의 한 형태로, 오류 정정을 통해, 공간(전자 통신)이나 시간(기억 장치) 속에서 송신된 자료의 무결성을 보호하는 단순한 방법이다
* TCP is a connection-oriented
* UDP is a datagram-oriented protocol


## 10) You want to implement a mechanism that automates the IP configuration, including IP address, subnet mask, default gateway, and DNS information. Which protocol will you use to accomplish this?
###   KEY)  DHCP
* DHCP란? ip주소를 동적으로 할당해주는 프로토콜.
* ip주소에 고정 아이피와 동적 아이피가 있다고 했는데, 동적 아이피가 DHCP와 관련 된 것.
* ARP: 네트워크 상에서 IP 주소를 물리적 네트워크 주소로 대응(bind)시키기 위해 사용되는 프로토콜. DHCP는 물리적 네트워크 주소가 아니라, IP주소를 할당해주기 위한 프로토콜.
* SNMP : 간이 망 관리 프로토콜(Simple Network Management Protocol, SNMP)은 IP 네트워크상의 장치로부터 정보를 수집 및 관리하며, 또한 정보를 수정하여 장치의 동작을 변경하는 데에 사용되는 인터넷 표준 프로토콜이다
* SMTP(Simple Mail Transfer Protocol): mail 전송 프로토콜. 데이터 전송의 신뢰성, 흐름 중요. TCP를 사용한다.

## 11) Which class of IP address has the most host addresses available by default?
###   KEY)  A
* A class 가 호스트 주소 영역 24bit(2^24-2개)

## 12) What is the Network address of a host with an IP address of 252.117.236.144/23?
###   KEY)  252.117.236.0
* 11111111.11111111.11111110.0 & 252.117.236.144
* network address : 252.117.236.0(252.117.11101100.0)


## 13) Which of the following is the valid host range for the subnet on which the IP address 227.109.176.237/26 resides?
###   KEY)  227.109.176.193-227.109.176.254
* 11111111.11111111.11111111.11000000 & 227.109.176.237
* network address : 227.109.176.192(227.109.176.11000000)
* broadcast address : 227.109.176.255(227.109.176.11111111)


## 14) What is the maximum number of IP addresses that can be assigned to hosts on a local subnet that uses the 255.0.0.0 subnet mask?
###   KEY)  16777214
* 2^24 - 2

## 15) How long is an IPv4 address?
###   KEY)  32 bits
* IPv6 = 128bits

## 16) Which of this is not true?
###   KEY)  TCP supports Broadcasting
* TCP는 무조건 1:1 연결.
* TCP는 연결지향적. 신뢰성을 중시한다.
* TCP provides extensive error checking mechanisms. It is because it provides 'flow control and acknowledgment of data'
* UDP = checksum - basic error check


## 17) What is the default subnet mask for a class C network?
###   KEY)  255.255.255.0
* A class 255.0.0.0
* B class 255.255.0.0
* C class 255.255.255.0

## 18) Which protocol does DHCP use at the Transport layer?
###   KEY)  UDP
* DHCP: DHCP 서버를 사용하여 IP 주소 및 관련된 기타 구성 세부 정보를 네트워크의 DHCP 사용 클라이언트에게 동적으로 할당하는 방법을 제공한다.
* UDP: 맞는 답이다. https://networkengineering.stackexchange.com/questions/64401/why-does-dhcp-use-udp-and-not-tcp
* TCP: 1:1 연결이 돼야 한다. ip주소가 없는 상황에서 ip주소를 동적으로 할당시켜 주는 것이기 때문에, ip주소:ip주소 1:1연결이 DHCP에서는 불가능 하다. 그래서 답이 아니다.
* IP: DHCP가 ip를 자동으로 할당해 주기 위한 프로토콜.
* ARP: 네트워크 상에서 IP 주소를 물리적 네트워크 주소로 대응(bind)시키기 위해 사용되는 프로토콜. DHCP는 물리적 네트워크 주소가 아니라, IP주소를 할당해주기 위한 프로토콜.

## 19) To test the IP stack on your local host, which IP address would you ping?
###   KEY)  127.0.0.1
* 로컬 호스트의 ip를 묻는 문제이다.
* 거의 모든 컴퓨터환경에서 자기 자신을 접근하는(loopback 이라고 한다고 함) 경우가 잦다. -> ping localhost 또는 ping 127.0.0.1 로 확인한다. https://velog.io/@taypark/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-%EA%B8%B0%EB%B3%B8-ping
* 그리하여 OS 자체적으로 제공하고 , 항상 고정되어 있는 IP(127.0.0.1) 과 호스트네임(localhost)을 갖는다.
* 127.0.0.1은 예약된 IP 주소로 인터넷상에 일반 IP로는 쓰일 수 없는 주소이다.
* OS에서 가상으로 지원하며, 랜카드 등 디바이스 자체를 통과하지 않고 소프트웨어적으로 처리된다.

## 20) If an Ethernet port on a router were assigned an IP address of 246.140.119.99/29, which host address would be able to communicate with it?
###   KEY)  246.140.119.97
* 11111111.11111111.11111111.11111000 & 246.140.119.99
* network address : 246.140.119.96(246.140.119.01100000)
* broadcast address : 246.140.119.127(246.140.119.01111111)
