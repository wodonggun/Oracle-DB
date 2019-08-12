https://raccoonjy.tistory.com/category/%EC%98%A4%EB%9D%BC%ED%81%B4DB


# sql 관련 명령

1. sqlplus를 실행한다.
로그인 ID : system  
비밀번호 : 설치시 비밀번호  

2. 유저 상태 명령어 : `SELECT username, account_status, lock_date FROM dba_users;`
EXPIRED & LOCKED로 나온 유저는 잠긴거.

3. 유저 잠김 해제 - `ALTER USER scott ACCOUNT UNLOCK;`

4. 유저 잠금 - `ALTER USER scott ACCOUNT LOCK;`


# 
