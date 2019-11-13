# Total 4 number of tests can be done on csrf

1. Simple CSRF
2. Anti CSRF token bypass
3. CSRF Content-Type:text/plain
4. CSRF FLASH

# 1. Simple CSRF Testing Methodology

1. Check if the given api endpoint is cookie based endpoint. </br>
&nbsp;&nbsp;&nbsp;It must be cookie based. </br>

2. Check if</br> 
****origin**** and ****referrer**** </br>
header are not validated by server by deleting and resending the request. </br>
> Origin: http://fl4tswa8w0y12jpm-apillab1.labs.peritustrainingschool.com </br>
> Referer: http://fl4tswa8w0y12jpm-apillab1.labs.peritustrainingschool.com/Csrf1 </br> </br>

&nbsp;&nbsp;&nbsp;They must not be validated by server.</br>

3. If server is not validating... :smiley:  </br>

4. **Exploit it.** </br>

> Note: you can generate poc from burp.

# 2. Testing when Anti CSRF Tockens are enabled.

> Note: Please check all tests by changing request methods also. </br>
1. First, check by passing blank parameter value. Check if server accepts. (Use burp and remove token value) </br>
> Token : Blank_Value </br>

2. Second, Remove parameter and anti-CSRF token completely. </br>

3. Add similar length token. (Change few values in token).</br>

4. Add another user’s valid anti-CSRF token. </br>

# 3. CSRF Content-Type:text/plain

1. Check if no anti-csrf tokens are used. If anti-csrf token is present try anti-csrf token bypass test.
2. Set `content-type=text/plain` and verify if the server is processing the request.
3. Exploitable.
