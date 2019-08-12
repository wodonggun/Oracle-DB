select * 
from emp E
    ,dept D 
where e.deptno = d.deptno 
  AND SAL <= 2500
  AND E.empno <= 9999 
ORDER BY SAL;





select * 
from emp E
    ,dept D 
where SAL <= 2500
  AND E.empno <= 9999 
ORDER BY SAL;

SELECT * FROM EMP A, SALGRADE B
WHERE A.SAL < B.hisal
AND A.SAL > B.losal
ORDER BY A.SAL; 


SELECT A.empno, A.ENAME, A.MGR, b.empno, b.ename
FROM EMP A, EMP B
WHERE A.mgr = B.empno(+);


select * fROm all_tab_columns where table_name = 'EMP';

select * from EMP where ename = 'KING';



SELECT * FROM ALL_TAB_COLUMNS 
WHERE COLUMN_NAME LIKE '%SAL%';


SELECT * FROM sdo_coord_op_param_use;




SELECT * FROM (
SELECT * FROM ALL_TAB_COLUMNS 
WHERE COLUMN_NAME LIKE '%SAL%')
WHERE OWNER = 'SYS';




SELECT * FROM SALGRADE;
