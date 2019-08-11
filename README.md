# Oracle-DB

# 오라클 아키텍처

1. 오라클 클라이언트
2. 오라클 서버 프로세스
3. 오라클 백그라운드 프로세스

오라클 클라이언트(java,c, sql developer 등 )는 오라클서버의 프로세스에 연결된다.   
프로세스 뒤에 백그라운드 프로세스는 프로세서가 동작하기 위해 보조 역할을 함.  

클라이언트(클라이언트 프로세스) - 서버(서버 프로세스) - 디스크  


- `오라클 서버` : 버퍼 캐시에 데이터 유무에 따라 1~2ms, 캐시에 데이터가 없을때 디스크를 거치게 되면 40ms정도 속도 차이가 발생함.



# 블록

오라클은 `블록`단위로 데이터를 가지고 오고, 저장함.  

- `PGA(Programing Global Area)` = 공유하지 않는 메모리 (각 서버프로세스 하나마다 독립적으로 가지고 있음)

- `SGA(System Global Area)` = 프로세스 끼리 공유하는 메모리 (A서버프로세스, B,C 모든 프로세스는 독립적으로 SGA를 가지고 있지만 서로 복사본 형태로 공유한다) 

SGA영역의 데이터 무결성을 위해 락(lock)을 걸고 사용함. 




# 세마포어

- 세마포어는 OS가 제공하는 자원관리를 하기 위한 장치
- 자원의 수에 비해 사용하고자 하는 프레소스의 수가 많을 경우 `순서대로 자원을 사용`할 수 있도록 제어 수행

