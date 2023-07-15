# oracle-apex-check-expire
oracle-apex-check-expire

```
select username, account_status, EXPIRY_DATE 
from dba_users 
where username in ('APEX_LISTENER','APEX_PUBLIC_USER','APEX_REST_PUBLIC_USER');
```

sample output:
```
USERNAME		       ACCOUNT_STATUS			EXPIRY_DA
------------------------------ -------------------------------- ---------
APEX_LISTENER		       OPEN				03-OCT-21
APEX_PUBLIC_USER	       OPEN				03-OCT-21
APEX_REST_PUBLIC_USER	       OPEN				03-OCT-21
```

another sample output:
```
USERNAME		       ACCOUNT_STATUS			EXPIRY_DA
------------------------------ -------------------------------- ---------
APEX_PUBLIC_USER	       OPEN				03-OCT-21
APEX_LISTENER		       EXPIRED				06-APR-21
APEX_REST_PUBLIC_USER	       EXPIRED				06-APR-21
```
