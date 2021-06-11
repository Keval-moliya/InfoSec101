# PicoGym Web Exploitation Writeup

Author: [Keval Moliya](https://github.com/Keval-moliya)

Challenge Page: [logon](https://jupiter.challenges.picoctf.org/problem/15796/)
## Walkthrough
First I tried SQL injection, didn't work.

Then I intercepted the HTTP request using Burp Suite, it only used to check for password if the username was Joe otherwise it would login in for any other username, so first entering some random username and password, on the GET request for `/flag` page we get this line:

`Cookie: PHPSESSID=vou3mgg3p3p432ekstq47bvpgb; password=admin; username=admin; admin=False`

So I changed the `username` and `admin` field to `Joe` and `True` respectively.

So yay!


## Flag
`picoCTF{th3_c0nsp1r4cy_l1v3s_6edb3f5f}`

## Useful resources (if any)
https://www.hacksplaining.com/exercises/sql-injection