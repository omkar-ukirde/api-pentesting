<h1> XXE Pentesting Methodology</h1>  

<p><pre><h2>1. XXE XML Entity Injection</h3>
<h4>1. Testing Viewable Injection</h4> 
      1. Search for api end points and change Content-Type to 
      <b>application/xml</b> 
        or 
      <b>text/xml</b> 
      and see if it is accepting xml.
      2. check if we can use internal entities.
      3. Check if we can use external entities using system keyword.
      4. inject into viewable parameter.
   
   
<h4>2. Testing Unviewable Injection</h4> 
      1. Search for api end points and change Content-Type to 
      <b>application/xml</b> 
        or 
      <b>text/xml</b> 
      and see if it is accepting xml.
      2. check if we can use internal entities.
      3. Check if we can use external entities using system keyword.
      4. send data to our out band server.</pre></p> 
    
<pre><h2>2. Simple Way to confirm XXE.</h3>  
    Use pingb.in to check if we can receive external ping.</pre>
    

<pre><h2>3. How it is patched</h3>
1. Block DTD
2. Block SYSTEM
3. Block specific URI's like file:/// http:// etc.
</pre>

<pre><h2>4. How it can be bypassed</h3>
1. Use FTP to perform OOB data extraction
2. Use php:// to get RCE or exploit XXE
3. Use gopher or other URI handlers.
</pre>

<pre><h2>5. Learn more indepth about xxe by labs on web-security by portswigger xxe exercise.</h3></pre>  
