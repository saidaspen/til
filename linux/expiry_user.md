# How to disable password aging for an user account

To turn off the password expiration for an user account, set the following:

- -m 0 will set the minimum number of days between password change to 0
- -M 99999 will set the maximum number of days between password change to 99999
- -I -1 (number minus one) will set the “Password inactive” to never
- -E -1 (number minus one) will set “Account expires” to never.

```
# chage -m 0 -M 99999 -I -1 -E -1 dhinesh

# chage --list dhinesh
Last password change                                    : Apr 23, 2009
Password expires                                        : never
Password inactive                                       : never
Account expires                                         : never
Minimum number of days between password change          : 0
Maximum number of days between password change          : 99999
Number of days of warning before password expires       : 7
```


