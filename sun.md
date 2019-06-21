
# ZAP Scanning Report




## Summary of Alerts

| Risk Level | Number of Alerts |
| --- | --- |
| High | 1 |
| Medium | 2 |
| Low | 7 |
| Informational | 0 |

## Alert Detail


  
  
  
### Viewstate without MAC Signature (Unsure)
##### High (Low)
  
  
  
  
#### Description
<p>*** EXPERIMENTAL ***</p><p>This website uses ASP.NET's Viewstate but maybe without any MAC.</p><p></p><p></p>
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `POST`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `GET`
  
  
  
  
Instances: 2
  
### Solution
<p>Ensure the MAC is set for all pages on this website.</p>
  
### Reference
* http://msdn.microsoft.com/en-us/library/ff649308.aspx

  
#### CWE Id : 642
  
#### WASC Id : 14
  
#### Source ID : 3

  
  
  
### X-Frame-Options Header Not Set
##### Medium (Medium)
  
  
  
  
#### Description
<p>X-Frame-Options header is not included in the HTTP response to protect against 'ClickJacking' attacks.</p>
  
  
  
* URL: [https://www.gstatic.com/chrome/intelligence/assist/ranker/models/translate/2017/03/translate_ranker_model_20170329.pb.bin](https://www.gstatic.com/chrome/intelligence/assist/ranker/models/translate/2017/03/translate_ranker_model_20170329.pb.bin)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
Instances: 1
  
### Solution
<p>Most modern Web browsers support the X-Frame-Options HTTP header. Ensure it's set on all web pages returned by your site (if you expect the page to be framed only by pages on your server (e.g. it's part of a FRAMESET) then you'll want to use SAMEORIGIN, otherwise if you never expect the page to be framed, you should use DENY. ALLOW-FROM allows specific websites to frame the web page in supported web browsers).</p>
  
### Reference
* http://blogs.msdn.com/b/ieinternals/archive/2010/03/30/combating-clickjacking-with-x-frame-options.aspx

  
#### CWE Id : 16
  
#### WASC Id : 15
  
#### Source ID : 3

  
  
  
### X-Frame-Options Header Not Set
##### Medium (Medium)
  
  
  
  
#### Description
<p>X-Frame-Options header is not included in the HTTP response to protect against 'ClickJacking' attacks.</p>
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
Instances: 2
  
### Solution
<p>Most modern Web browsers support the X-Frame-Options HTTP header. Ensure it's set on all web pages returned by your site (if you expect the page to be framed only by pages on your server (e.g. it's part of a FRAMESET) then you'll want to use SAMEORIGIN, otherwise if you never expect the page to be framed, you should use DENY. ALLOW-FROM allows specific websites to frame the web page in supported web browsers).</p>
  
### Reference
* http://blogs.msdn.com/b/ieinternals/archive/2010/03/30/combating-clickjacking-with-x-frame-options.aspx

  
#### CWE Id : 16
  
#### WASC Id : 15
  
#### Source ID : 3

  
  
  
### Web Browser XSS Protection Not Enabled
##### Low (Medium)
  
  
  
  
#### Description
<p>Web Browser XSS Protection is not enabled, or is disabled by the configuration of the 'X-XSS-Protection' HTTP response header on the web server</p>
  
  
  
* URL: [https://www.gstatic.com/chrome/intelligence/assist/ranker/models/translate/2017/03/translate_ranker_model_20170329.pb.bin](https://www.gstatic.com/chrome/intelligence/assist/ranker/models/translate/2017/03/translate_ranker_model_20170329.pb.bin)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  * Evidence: `X-XSS-Protection: 0`
  
  
  
  
Instances: 1
  
### Solution
<p>Ensure that the web browser's XSS filter is enabled, by setting the X-XSS-Protection HTTP response header to '1'.</p>
  
### Other information
<p>The X-XSS-Protection HTTP response header allows the web server to enable or disable the web browser's XSS protection mechanism. The following values would attempt to enable it: </p><p>X-XSS-Protection: 1; mode=block</p><p>X-XSS-Protection: 1; report=http://www.example.com/xss</p><p>The following values would disable it:</p><p>X-XSS-Protection: 0</p><p>The X-XSS-Protection HTTP response header is currently supported on Internet Explorer, Chrome and Safari (WebKit).</p><p>Note that this alert is only raised if the response body could potentially contain an XSS payload (with a text-based content type, with a non-zero length).</p>
  
### Reference
* https://www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet
* https://www.veracode.com/blog/2014/03/guidelines-for-setting-security-headers/

  
#### CWE Id : 933
  
#### WASC Id : 14
  
#### Source ID : 3

  
  
  
### Incomplete or No Cache-control and Pragma HTTP Header Set
##### Low (Medium)
  
  
  
  
#### Description
<p>The cache-control and pragma HTTP header have not been set properly or are missing allowing the browser and proxies to cache content.</p>
  
  
  
* URL: [https://www.gstatic.com/chrome/intelligence/assist/ranker/models/translate/2017/03/translate_ranker_model_20170329.pb.bin](https://www.gstatic.com/chrome/intelligence/assist/ranker/models/translate/2017/03/translate_ranker_model_20170329.pb.bin)
  
  
  * Method: `GET`
  
  
  * Parameter: `Cache-Control`
  
  
  * Evidence: `public, max-age=31536000`
  
  
  
  
Instances: 1
  
### Solution
<p>Whenever possible ensure the cache-control HTTP header is set with no-cache, no-store, must-revalidate; and that the pragma HTTP header is set with no-cache.</p>
  
### Reference
* https://www.owasp.org/index.php/Session_Management_Cheat_Sheet#Web_Content_Caching

  
#### CWE Id : 525
  
#### WASC Id : 13
  
#### Source ID : 3

  
  
  
### Web Browser XSS Protection Not Enabled
##### Low (Medium)
  
  
  
  
#### Description
<p>Web Browser XSS Protection is not enabled, or is disabled by the configuration of the 'X-XSS-Protection' HTTP response header on the web server</p>
  
  
  
* URL: [http://sunsmart.in/robots.txt](http://sunsmart.in/robots.txt)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/js/jquery.slides.min.js](http://sunsmart.in/mydesk/smartadmin/js/jquery.slides.min.js)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://sunsmart.in/sitemap.xml](http://sunsmart.in/sitemap.xml)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/%22%20+%20imageArray%5Brand%5D%20+%20%22](http://sunsmart.in/mydesk/smartadmin/%22%20+%20imageArray%5Brand%5D%20+%20%22)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
Instances: 6
  
### Solution
<p>Ensure that the web browser's XSS filter is enabled, by setting the X-XSS-Protection HTTP response header to '1'.</p>
  
### Other information
<p>The X-XSS-Protection HTTP response header allows the web server to enable or disable the web browser's XSS protection mechanism. The following values would attempt to enable it: </p><p>X-XSS-Protection: 1; mode=block</p><p>X-XSS-Protection: 1; report=http://www.example.com/xss</p><p>The following values would disable it:</p><p>X-XSS-Protection: 0</p><p>The X-XSS-Protection HTTP response header is currently supported on Internet Explorer, Chrome and Safari (WebKit).</p><p>Note that this alert is only raised if the response body could potentially contain an XSS payload (with a text-based content type, with a non-zero length).</p>
  
### Reference
* https://www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet
* https://www.veracode.com/blog/2014/03/guidelines-for-setting-security-headers/

  
#### CWE Id : 933
  
#### WASC Id : 14
  
#### Source ID : 3

  
  
  
### X-Content-Type-Options Header Missing
##### Low (Medium)
  
  
  
  
#### Description
<p>The Anti-MIME-Sniffing header X-Content-Type-Options was not set to 'nosniff'. This allows older versions of Internet Explorer and Chrome to perform MIME-sniffing on the response body, potentially causing the response body to be interpreted and displayed as a content type other than the declared content type. Current (early 2014) and legacy versions of Firefox will use the declared content type (if one is set), rather than performing MIME-sniffing.</p>
  
  
  
* URL: [http://sunsmart.in/mydesk/Indexpage2css/bootstrap/js/bootstrap.min.js](http://sunsmart.in/mydesk/Indexpage2css/bootstrap/js/bootstrap.min.js)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/Images/ntireoffice_new-1.png](http://sunsmart.in/mydesk/smartadmin/Images/ntireoffice_new-1.png)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/Mydesk/WebResource.axd?d=fG8idjXK-sRCYwyd8uDHW_1FhmtwqLJC2lMFL9nO3WK21S1dfDmUivFsyt-kJF4aPTWJyL3IiRWYS6cLX5jCspPh20jkzQeo9GK03wbfhww1&t=636577232940000000](http://sunsmart.in/Mydesk/WebResource.axd?d=fG8idjXK-sRCYwyd8uDHW_1FhmtwqLJC2lMFL9nO3WK21S1dfDmUivFsyt-kJF4aPTWJyL3IiRWYS6cLX5jCspPh20jkzQeo9GK03wbfhww1&t=636577232940000000)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/js/md5.js](http://sunsmart.in/mydesk/smartadmin/js/md5.js)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/js/jsencryptionform.js](http://sunsmart.in/mydesk/smartadmin/js/jsencryptionform.js)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/Indexpage2css/bootstrap/css/bootstrap.min.css](http://sunsmart.in/mydesk/Indexpage2css/bootstrap/css/bootstrap.min.css)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/js/jquery-1.10.2.js](http://sunsmart.in/mydesk/smartadmin/js/jquery-1.10.2.js)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/Mydesk/WebResource.axd?d=8Y8EvT9lYGpRU58CJVvDZw3TaUfKXgRRjemtoHmayWuq0X-FYiN4OWNc2pHwEo-Hk1bqDJHBNBMUKjNL7CxtXX-qsjoYn8YKpY0an8SmjvI1&t=636577232940000000](http://sunsmart.in/Mydesk/WebResource.axd?d=8Y8EvT9lYGpRU58CJVvDZw3TaUfKXgRRjemtoHmayWuq0X-FYiN4OWNc2pHwEo-Hk1bqDJHBNBMUKjNL7CxtXX-qsjoYn8YKpY0an8SmjvI1&t=636577232940000000)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/Mydesk/ScriptResource.axd?d=JKiZGkqhBX5XimDh14W3FB5NudX1_BBf_HaKZMXKQLCCjZFg8wEr0QxN7-Gg3M4uZzovkh1JfXbev981CSIoDRSDcQAbVEExTCe5Yd7-jiVBVq5JuDqVijtqam7y-0ATs6bLhefT1Ul_r2P60XWgaU_2aQFzZYlAJkuQzayT6VpQkifG7StV5viOL4DSCtc80&t=ffffffffcd368728](http://sunsmart.in/Mydesk/ScriptResource.axd?d=JKiZGkqhBX5XimDh14W3FB5NudX1_BBf_HaKZMXKQLCCjZFg8wEr0QxN7-Gg3M4uZzovkh1JfXbev981CSIoDRSDcQAbVEExTCe5Yd7-jiVBVq5JuDqVijtqam7y-0ATs6bLhefT1Ul_r2P60XWgaU_2aQFzZYlAJkuQzayT6VpQkifG7StV5viOL4DSCtc80&t=ffffffffcd368728)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/js/BrowserClose.js](http://sunsmart.in/mydesk/smartadmin/js/BrowserClose.js)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/Mydesk/ScriptResource.axd?d=4x3qheOz1bPixdJzZdXYVqRc3H6ZLGWgdnEhMNRMUBPtyOHfguzNTx2j232UiIX6U7Q6x-3EwWIGatwW0uqD5w0LG6WvoZilY47ukGhdlPF4wJOPKDpU7WwgpaBHNcE9Z6MJ9J7Znc7jHsZZrHLssun3M63vHaA9KPL03f9ZthTDfJTtdtV8ko4ZkVm_4Jd30&t=ffffffffcd368728](http://sunsmart.in/Mydesk/ScriptResource.axd?d=4x3qheOz1bPixdJzZdXYVqRc3H6ZLGWgdnEhMNRMUBPtyOHfguzNTx2j232UiIX6U7Q6x-3EwWIGatwW0uqD5w0LG6WvoZilY47ukGhdlPF4wJOPKDpU7WwgpaBHNcE9Z6MJ9J7Znc7jHsZZrHLssun3M63vHaA9KPL03f9ZthTDfJTtdtV8ko4ZkVm_4Jd30&t=ffffffffcd368728)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/js/jquery.min.js](http://sunsmart.in/mydesk/smartadmin/js/jquery.min.js)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/js/common.js](http://sunsmart.in/mydesk/smartadmin/js/common.js)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/Images/loading.png](http://sunsmart.in/mydesk/smartadmin/Images/loading.png)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/LoginImages/minilogo.png](http://sunsmart.in/mydesk/smartadmin/LoginImages/minilogo.png)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/js/jsencryption.js](http://sunsmart.in/mydesk/smartadmin/js/jsencryption.js)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
Instances: 18
  
### Solution
<p>Ensure that the application/web server sets the Content-Type header appropriately, and that it sets the X-Content-Type-Options header to 'nosniff' for all web pages.</p><p>If possible, ensure that the end user uses a standards-compliant and modern web browser that does not perform MIME-sniffing at all, or that can be directed by the web application/web server to not perform MIME-sniffing.</p>
  
### Other information
<p>This issue still applies to error type pages (401, 403, 500, etc) as those pages are often still affected by injection issues, in which case there is still concern for browsers sniffing pages away from their actual content type.</p><p>At "High" threshold this scanner will not alert on client or server error responses.</p>
  
### Reference
* http://msdn.microsoft.com/en-us/library/ie/gg622941%28v=vs.85%29.aspx
* https://www.owasp.org/index.php/List_of_useful_HTTP_headers

  
#### CWE Id : 16
  
#### WASC Id : 15
  
#### Source ID : 3

  
  
  
### Application Error Disclosure
##### Low (Medium)
  
  
  
  
#### Description
<p>This page contains an error/warning message that may disclose sensitive information like the location of the file that produced the unhandled exception. This information can be used to launch further attacks against the web application. The alert could be a false positive if the error message is found inside a documentation page.</p>
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Internal Server Error`
  
  
  
  
Instances: 1
  
### Solution
<p>Review the source code of this page. Implement custom error pages. Consider implementing a mechanism to provide a unique error reference/identifier to the client (browser) while logging the details on the server side and not exposing them to the user.</p>
  
### Reference
* 

  
#### CWE Id : 200
  
#### WASC Id : 13
  
#### Source ID : 3

  
  
  
### Absence of Anti-CSRF Tokens
##### Low (Medium)
  
  
  
  
#### Description
<p>No Anti-CSRF tokens were found in a HTML submission form.</p><p>A cross-site request forgery is an attack that involves forcing a victim to send an HTTP request to a target destination without their knowledge or intent in order to perform an action as the victim. The underlying cause is application functionality using predictable URL/form actions in a repeatable way. The nature of the attack is that CSRF exploits the trust that a web site has for a user. By contrast, cross-site scripting (XSS) exploits the trust that a user has for a web site. Like XSS, CSRF attacks are not necessarily cross-site, but they can be. Cross-site request forgery is also known as CSRF, XSRF, one-click attack, session riding, confused deputy, and sea surf.</p><p></p><p>CSRF attacks are effective in a number of situations, including:</p><p>    * The victim has an active session on the target site.</p><p>    * The victim is authenticated via HTTP auth on the target site.</p><p>    * The victim is on the same local network as the target site.</p><p></p><p>CSRF has primarily been used to perform an action against a target site using the victim's privileges, but recent techniques have been discovered to disclose information by gaining access to the response. The risk of information disclosure is dramatically increased when the target site is vulnerable to XSS, because XSS can be used as a platform for CSRF, allowing the attack to operate within the bounds of the same-origin policy.</p>
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `POST`
  
  
  * Evidence: `<form name="frm" method="post" action="./smartlogin.aspx" onkeypress="javascript:return WebForm_FireDefaultButton(event, 'imggo1')" id="frm" autocomplete="off" style="height:100%">`
  
  
  
  
* URL: [http://sunsmart.in/Mydesk/WebResource.axd?d=8Y8EvT9lYGpRU58CJVvDZw3TaUfKXgRRjemtoHmayWuq0X-FYiN4OWNc2pHwEo-Hk1bqDJHBNBMUKjNL7CxtXX-qsjoYn8YKpY0an8SmjvI1&t=636577232940000000](http://sunsmart.in/Mydesk/WebResource.axd?d=8Y8EvT9lYGpRU58CJVvDZw3TaUfKXgRRjemtoHmayWuq0X-FYiN4OWNc2pHwEo-Hk1bqDJHBNBMUKjNL7CxtXX-qsjoYn8YKpY0an8SmjvI1&t=636577232940000000)
  
  
  * Method: `GET`
  
  
  * Evidence: `<form method="post">`
  
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `GET`
  
  
  * Evidence: `<form name="frm" method="post" action="./smartlogin.aspx" onkeypress="javascript:return WebForm_FireDefaultButton(event, 'imggo1')" id="frm" autocomplete="off" style="height:100%">`
  
  
  
  
Instances: 3
  
### Solution
<p>Phase: Architecture and Design</p><p>Use a vetted library or framework that does not allow this weakness to occur or provides constructs that make this weakness easier to avoid.</p><p>For example, use anti-CSRF packages such as the OWASP CSRFGuard.</p><p></p><p>Phase: Implementation</p><p>Ensure that your application is free of cross-site scripting issues, because most CSRF defenses can be bypassed using attacker-controlled script.</p><p></p><p>Phase: Architecture and Design</p><p>Generate a unique nonce for each form, place the nonce into the form, and verify the nonce upon receipt of the form. Be sure that the nonce is not predictable (CWE-330).</p><p>Note that this can be bypassed using XSS.</p><p></p><p>Identify especially dangerous operations. When the user performs a dangerous operation, send a separate confirmation request to ensure that the user intended to perform that operation.</p><p>Note that this can be bypassed using XSS.</p><p></p><p>Use the ESAPI Session Management control.</p><p>This control includes a component for CSRF.</p><p></p><p>Do not use the GET method for any request that triggers a state change.</p><p></p><p>Phase: Implementation</p><p>Check the HTTP Referer header to see if the request originated from an expected page. This could break legitimate functionality, because users or proxies may have disabled sending the Referer for privacy reasons.</p>
  
### Other information
<p>No known Anti-CSRF token [anticsrf, CSRFToken, __RequestVerificationToken, csrfmiddlewaretoken, authenticity_token, OWASP_CSRFTOKEN, anoncsrf, csrf_token, _csrf, _csrfSecret] was found in the following HTML form: [Form 1: "__EVENTTARGET" "__EVENTARGUMENT" "__VIEWSTATE" "__VIEWSTATEGENERATOR" "__EVENTVALIDATION" "hfimg" "txtUserID" "txtmainpassword" "txtPassword" "Accountlogindropdown" "chkremember" "btnmail" "imgGO" "imggo1" "btnsession" "Hfencript" "Hfpwdold" "sessionvalue" "hdnfuncDesc" "hidden1" "hidden2" "hfBrowserName" "hfBrowserVersion" ].</p>
  
### Reference
* http://projects.webappsec.org/Cross-Site-Request-Forgery
* http://cwe.mitre.org/data/definitions/352.html

  
#### CWE Id : 352
  
#### WASC Id : 9
  
#### Source ID : 3

  
  
  
### Information Disclosure - Debug Error Messages
##### Low (Medium)
  
  
  
  
#### Description
<p>The response appeared to contain common error messages returned by platforms such as ASP.NET, and Web-servers such as IIS and Apache. You can configure the list of common debug messages.</p>
  
  
  
* URL: [http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx](http://sunsmart.in/mydesk/smartadmin/smartlogin.aspx)
  
  
  * Method: `POST`
  
  
  * Evidence: `customErrors mode`
  
  
  
  
Instances: 1
  
### Solution
<p>Disable debugging messages before pushing to production.</p>
  
### Reference
* 

  
#### CWE Id : 200
  
#### WASC Id : 13
  
#### Source ID : 3
