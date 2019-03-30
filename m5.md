
# ZAP Scanning Report




## Summary of Alerts

| Risk Level | Number of Alerts |
| --- | --- |
| High | 0 |
| Medium | 3 |
| Low | 2 |
| Informational | 0 |

## Alert Detail


  
  
  
### Application Error Disclosure
##### Medium (Medium)
  
  
  
  
#### Description
<p>This page contains an error/warning message that may disclose sensitive information like the location of the file that produced the unhandled exception. This information can be used to launch further attacks against the web application. The alert could be a false positive if the error message is found inside a documentation page.</p>
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/?q=user/password/](http://testcrewpoint.caddcentre.com/?q=user/password/)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/themes/%2A.css%24?destination=themes/%2A.css%24](http://testcrewpoint.caddcentre.com/themes/%2A.css%24?destination=themes/%2A.css%24)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/modules/%2A.js%24?destination=modules/%2A.js%24](http://testcrewpoint.caddcentre.com/modules/%2A.js%24?destination=modules/%2A.js%24)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/node/470?destination=node/1](http://testcrewpoint.caddcentre.com/node/470?destination=node/1)
  
  
  * Method: `GET`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/?q=user/register/](http://testcrewpoint.caddcentre.com/?q=user/register/)
  
  
  * Method: `GET`
  
  
  * Evidence: `HTTP/1.1 500 Internal Server Error`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/node/470?destination=node/1](http://testcrewpoint.caddcentre.com/node/470?destination=node/1)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/user/register/](http://testcrewpoint.caddcentre.com/user/register/)
  
  
  * Method: `GET`
  
  
  * Evidence: `HTTP/1.1 500 Internal Server Error`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/themes/?destination=themes](http://testcrewpoint.caddcentre.com/themes/?destination=themes)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/modules/?destination=modules](http://testcrewpoint.caddcentre.com/modules/?destination=modules)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/user/password/](http://testcrewpoint.caddcentre.com/user/password/)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/includes/?destination=includes](http://testcrewpoint.caddcentre.com/includes/?destination=includes)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/node/470?destination=search](http://testcrewpoint.caddcentre.com/node/470?destination=search)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/misc/?destination=misc](http://testcrewpoint.caddcentre.com/misc/?destination=misc)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/user/register](http://testcrewpoint.caddcentre.com/user/register)
  
  
  * Method: `GET`
  
  
  * Evidence: `HTTP/1.1 500 Internal Server Error`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/sitemap.xml?destination=sitemap.xml](http://testcrewpoint.caddcentre.com/sitemap.xml?destination=sitemap.xml)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/filter/tips?destination=filter/tips](http://testcrewpoint.caddcentre.com/filter/tips?destination=filter/tips)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/cron.php?destination=cron.php](http://testcrewpoint.caddcentre.com/cron.php?destination=cron.php)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/node/470?destination=admin](http://testcrewpoint.caddcentre.com/node/470?destination=admin)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/misc/%2A.js%24?destination=misc/%2A.js%24](http://testcrewpoint.caddcentre.com/misc/%2A.js%24?destination=misc/%2A.js%24)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/profiles/%2A.css%24?destination=profiles/%2A.css%24](http://testcrewpoint.caddcentre.com/profiles/%2A.css%24?destination=profiles/%2A.css%24)
  
  
  * Method: `POST`
  
  
  * Evidence: `HTTP/1.1 500 Service unavailable (with message)`
  
  
  
  
Instances: 30
  
### Solution
<p>Review the source code of this page. Implement custom error pages. Consider implementing a mechanism to provide a unique error reference/identifier to the client (browser) while logging the details on the server side and not exposing them to the user.</p>
  
### Reference
* 

  
#### CWE Id : 200
  
#### WASC Id : 13
  
#### Source ID : 3

  
  
  
### X-Frame-Options Header Not Set
##### Medium (Medium)
  
  
  
  
#### Description
<p>X-Frame-Options header is not included in the HTTP response to protect against 'ClickJacking' attacks.</p>
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/xmlrpc.php](http://testcrewpoint.caddcentre.com/xmlrpc.php)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/install.php](http://testcrewpoint.caddcentre.com/install.php)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/php_files/tour_summary/ajax/tourAdvance_printView.php?id=10&sendid=2202&dept=SSG](http://testcrewpoint.caddcentre.com/php_files/tour_summary/ajax/tourAdvance_printView.php?id=10&sendid=2202&dept=SSG)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
Instances: 3
  
### Solution
<p>Most modern Web browsers support the X-Frame-Options HTTP header. Ensure it's set on all web pages returned by your site (if you expect the page to be framed only by pages on your server (e.g. it's part of a FRAMESET) then you'll want to use SAMEORIGIN, otherwise if you never expect the page to be framed, you should use DENY. ALLOW-FROM allows specific websites to frame the web page in supported web browsers).</p>
  
### Reference
* http://blogs.msdn.com/b/ieinternals/archive/2010/03/30/combating-clickjacking-with-x-frame-options.aspx

  
#### CWE Id : 16
  
#### WASC Id : 15
  
#### Source ID : 3

  
  
  
### Parameter Tampering
##### Medium (Low)
  
  
  
  
#### Description
<p>Parameter manipulation caused an error page or Java stack trace to be displayed.  This indicated lack of exception handling and potential areas for further exploit.</p>
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/php_files/tour_summary/ajax/tourAdvance_printView.php?=&sendid=2202&dept=SSG](http://testcrewpoint.caddcentre.com/php_files/tour_summary/ajax/tourAdvance_printView.php?=&sendid=2202&dept=SSG)
  
  
  * Method: `GET`
  
  
  * Parameter: `id`
  
  
  * Evidence: ` on line <b>`
  
  
  
  
Instances: 1
  
### Solution
<p>Identify the cause of the error and fix it.  Do not trust client side input and enforce a tight check in the server side.  Besides, catch the exception properly.  Use a generic 500 error page for internal server error.</p>
  
### Reference
* 

  
#### CWE Id : 472
  
#### WASC Id : 20
  
#### Source ID : 1

  
  
  
### Web Browser XSS Protection Not Enabled
##### Low (Medium)
  
  
  
  
#### Description
<p>Web Browser XSS Protection is not enabled, or is disabled by the configuration of the 'X-XSS-Protection' HTTP response header on the web server</p>
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/profiles/*.css$](http://testcrewpoint.caddcentre.com/profiles/*.css$)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/user/register/](http://testcrewpoint.caddcentre.com/user/register/)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/sitemap.xml?destination=sitemap.xml](http://testcrewpoint.caddcentre.com/sitemap.xml?destination=sitemap.xml)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/misc/*.js$](http://testcrewpoint.caddcentre.com/misc/*.js$)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/modules/](http://testcrewpoint.caddcentre.com/modules/)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/modules/](http://testcrewpoint.caddcentre.com/modules/)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/misc/%2A.js%24?destination=misc/%2A.js%24](http://testcrewpoint.caddcentre.com/misc/%2A.js%24?destination=misc/%2A.js%24)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/profiles/*.css$](http://testcrewpoint.caddcentre.com/profiles/*.css$)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/misc/?destination=misc](http://testcrewpoint.caddcentre.com/misc/?destination=misc)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/cron.php](http://testcrewpoint.caddcentre.com/cron.php)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/profiles/*.png](http://testcrewpoint.caddcentre.com/profiles/*.png)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/modules/?destination=modules](http://testcrewpoint.caddcentre.com/modules/?destination=modules)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/themes/*.css$](http://testcrewpoint.caddcentre.com/themes/*.css$)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/scripts/](http://testcrewpoint.caddcentre.com/scripts/)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/?q=user/logout/](http://testcrewpoint.caddcentre.com/?q=user/logout/)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/?q=node/add/](http://testcrewpoint.caddcentre.com/?q=node/add/)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/misc/*.css$](http://testcrewpoint.caddcentre.com/misc/*.css$)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/node/470?destination=search](http://testcrewpoint.caddcentre.com/node/470?destination=search)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/filter/tips/](http://testcrewpoint.caddcentre.com/filter/tips/)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/scripts/](http://testcrewpoint.caddcentre.com/scripts/)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
Instances: 139
  
### Solution
<p>Ensure that the web browser's XSS filter is enabled, by setting the X-XSS-Protection HTTP response header to '1'.</p>
  
### Other information
<p>The X-XSS-Protection HTTP response header allows the web server to enable or disable the web browser's XSS protection mechanism. The following values would attempt to enable it: </p><p>X-XSS-Protection: 1; mode=block</p><p>X-XSS-Protection: 1; report=http://www.example.com/xss</p><p>The following values would disable it:</p><p>X-XSS-Protection: 0</p><p>The X-XSS-Protection HTTP response header is currently supported on Internet Explorer, Chrome and Safari (WebKit).</p><p>Note that this alert is only raised if the response body could potentially contain an XSS payload (with a text-based content type, with a non-zero length).</p>
  
### Reference
* https://www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet
* https://blog.veracode.com/2014/03/guidelines-for-setting-security-headers/

  
#### CWE Id : 933
  
#### WASC Id : 14
  
#### Source ID : 3

  
  
  
### X-Content-Type-Options Header Missing
##### Low (Medium)
  
  
  
  
#### Description
<p>The Anti-MIME-Sniffing header X-Content-Type-Options was not set to 'nosniff'. This allows older versions of Internet Explorer and Chrome to perform MIME-sniffing on the response body, potentially causing the response body to be interpreted and displayed as a content type other than the declared content type. Current (early 2014) and legacy versions of Firefox will use the declared content type (if one is set), rather than performing MIME-sniffing.</p>
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/misc/drupal.js?pmljti](http://testcrewpoint.caddcentre.com/misc/drupal.js?pmljti)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/LICENSE.txt](http://testcrewpoint.caddcentre.com/LICENSE.txt)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/sites/all/modules/nice_menus-7.x-2.1/nice_menus/superfish/js/superfish.js?pmljti](http://testcrewpoint.caddcentre.com/sites/all/modules/nice_menus-7.x-2.1/nice_menus/superfish/js/superfish.js?pmljti)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/themes/seven/ie7.css?pmljti](http://testcrewpoint.caddcentre.com/themes/seven/ie7.css?pmljti)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/php_files/images/cadd_25_years.png](http://testcrewpoint.caddcentre.com/php_files/images/cadd_25_years.png)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/themes/seven/ie6.css?pmljti](http://testcrewpoint.caddcentre.com/themes/seven/ie6.css?pmljti)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/themes/seven/ie.css?pmljti](http://testcrewpoint.caddcentre.com/themes/seven/ie.css?pmljti)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/MAINTAINERS.txt](http://testcrewpoint.caddcentre.com/MAINTAINERS.txt)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/sites/all/themes/corporateclean-7.x-1.4/corporateclean/js/jquery.cycle.all.min.js?pmljti](http://testcrewpoint.caddcentre.com/sites/all/themes/corporateclean-7.x-1.4/corporateclean/js/jquery.cycle.all.min.js?pmljti)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/sites/all/themes/corporateclean-7.x-1.4/corporateclean/logo.png](http://testcrewpoint.caddcentre.com/sites/all/themes/corporateclean-7.x-1.4/corporateclean/logo.png)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/misc/tableheader.js?pmljti](http://testcrewpoint.caddcentre.com/misc/tableheader.js?pmljti)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/misc/favicon.ico](http://testcrewpoint.caddcentre.com/misc/favicon.ico)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/sites/all/modules/nice_menus-7.x-2.1/nice_menus/nice_menus.js?pmljti](http://testcrewpoint.caddcentre.com/sites/all/modules/nice_menus-7.x-2.1/nice_menus/nice_menus.js?pmljti)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/CHANGELOG.txt](http://testcrewpoint.caddcentre.com/CHANGELOG.txt)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/sites/all/themes/corporateclean-7.x-1.4/corporateclean/js/user-registerform.js?pmljti](http://testcrewpoint.caddcentre.com/sites/all/themes/corporateclean-7.x-1.4/corporateclean/js/user-registerform.js?pmljti)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/INSTALL.txt](http://testcrewpoint.caddcentre.com/INSTALL.txt)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/INSTALL.sqlite.txt](http://testcrewpoint.caddcentre.com/INSTALL.sqlite.txt)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/sites/all/modules/captcha-7.x-1.3/captcha/captcha.js?pmljti](http://testcrewpoint.caddcentre.com/sites/all/modules/captcha-7.x-1.3/captcha/captcha.js?pmljti)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/misc/drupal.js?0](http://testcrewpoint.caddcentre.com/misc/drupal.js?0)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://testcrewpoint.caddcentre.com/php_files/cadd-center-logo.png](http://testcrewpoint.caddcentre.com/php_files/cadd-center-logo.png)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
Instances: 32
  
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
