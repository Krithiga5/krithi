
# ZAP Scanning Report




## Summary of Alerts

| Risk Level | Number of Alerts |
| --- | --- |
| High | 0 |
| Medium | 1 |
| Low | 2 |
| Informational | 0 |

## Alert Detail


  
  
  
### X-Frame-Options Header Not Set
##### Medium (Medium)
  
  
  
  
#### Description
<p>X-Frame-Options header is not included in the HTTP response to protect against 'ClickJacking' attacks.</p>
  
  
  
* URL: [http://supportlivewireindiacom.test3/online-leads](http://supportlivewireindiacom.test3/online-leads)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user?current=user/password](http://supportlivewireindiacom.test3/user?current=user/password)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user?current=user/password](http://supportlivewireindiacom.test3/user?current=user/password)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user](http://supportlivewireindiacom.test3/user)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user/login?destination=node/648](http://supportlivewireindiacom.test3/user/login?destination=node/648)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user/password](http://supportlivewireindiacom.test3/user/password)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user/password](http://supportlivewireindiacom.test3/user/password)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user/login?destination=node/648](http://supportlivewireindiacom.test3/user/login?destination=node/648)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user](http://supportlivewireindiacom.test3/user)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-Frame-Options`
  
  
  
  
Instances: 9
  
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
  
  
  
* URL: [http://supportlivewireindiacom.test3/user/password](http://supportlivewireindiacom.test3/user/password)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user/login?destination=node/648](http://supportlivewireindiacom.test3/user/login?destination=node/648)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user](http://supportlivewireindiacom.test3/user)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/node?destination=node](http://supportlivewireindiacom.test3/node?destination=node)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user/login?destination=node/648](http://supportlivewireindiacom.test3/user/login?destination=node/648)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user?current=user/password](http://supportlivewireindiacom.test3/user?current=user/password)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/online-leads](http://supportlivewireindiacom.test3/online-leads)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user?current=user/password](http://supportlivewireindiacom.test3/user?current=user/password)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/default/files/css/font-awesome.css](http://supportlivewireindiacom.test3/sites/default/files/css/font-awesome.css)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/](http://supportlivewireindiacom.test3/)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sitemap.xml](http://supportlivewireindiacom.test3/sitemap.xml)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user/password](http://supportlivewireindiacom.test3/user/password)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/user](http://supportlivewireindiacom.test3/user)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/node?destination=node](http://supportlivewireindiacom.test3/node?destination=node)
  
  
  * Method: `POST`
  
  
  * Parameter: `X-XSS-Protection`
  
  
  
  
Instances: 14
  
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
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/themes/flat-metro/js/foundation3/foundation.min.js?pqew54](http://supportlivewireindiacom.test3/sites/all/themes/flat-metro/js/foundation3/foundation.min.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/modules/colorbox/js/colorbox.js?pqew54](http://supportlivewireindiacom.test3/sites/all/modules/colorbox/js/colorbox.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/themes/flat-metro/js/responsiveslides.js?pqew54](http://supportlivewireindiacom.test3/sites/all/themes/flat-metro/js/responsiveslides.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/misc/ajax.js?v=7.43](http://supportlivewireindiacom.test3/misc/ajax.js?v=7.43)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/misc/drupal.js?pqew54](http://supportlivewireindiacom.test3/misc/drupal.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/robots.txt](http://supportlivewireindiacom.test3/robots.txt)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/themes/flat-metro/js/foundation/foundation.min.js?pqew54](http://supportlivewireindiacom.test3/sites/all/themes/flat-metro/js/foundation/foundation.min.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/modules/clientside_validation/jquery-validate/jquery.validate.js?pqew54](http://supportlivewireindiacom.test3/sites/all/modules/clientside_validation/jquery-validate/jquery.validate.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/modules/captcha/captcha/captcha.js?pqew54](http://supportlivewireindiacom.test3/sites/all/modules/captcha/captcha/captcha.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/themes/flat-metro/js/scripts.js?pqew54](http://supportlivewireindiacom.test3/sites/all/themes/flat-metro/js/scripts.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/modules/panels/js/panels.js?pqew54](http://supportlivewireindiacom.test3/sites/all/modules/panels/js/panels.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/themes/flat-metro/css/foundation3/foundation.css?pqew54](http://supportlivewireindiacom.test3/sites/all/themes/flat-metro/css/foundation3/foundation.css?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/libraries/colorbox/jquery.colorbox-min.js?pqew54](http://supportlivewireindiacom.test3/sites/all/libraries/colorbox/jquery.colorbox-min.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/modules/colorbox/styles/default/colorbox_style.js?pqew54](http://supportlivewireindiacom.test3/sites/all/modules/colorbox/styles/default/colorbox_style.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/default/files/logo.png](http://supportlivewireindiacom.test3/sites/default/files/logo.png)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/misc/jquery.once.js?v=1.2](http://supportlivewireindiacom.test3/misc/jquery.once.js?v=1.2)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/modules/jreject/jReject/js/jquery.reject.js?pqew54](http://supportlivewireindiacom.test3/sites/all/modules/jreject/jReject/js/jquery.reject.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/libraries/jstorage/jstorage.min.js?pqew54](http://supportlivewireindiacom.test3/sites/all/libraries/jstorage/jstorage.min.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/themes/zurb-foundation/js/vendor/custom.modernizr.js?pqew54](http://supportlivewireindiacom.test3/sites/all/themes/zurb-foundation/js/vendor/custom.modernizr.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
* URL: [http://supportlivewireindiacom.test3/sites/all/themes/zurb-foundation/js/foundation.min.js?pqew54](http://supportlivewireindiacom.test3/sites/all/themes/zurb-foundation/js/foundation.min.js?pqew54)
  
  
  * Method: `GET`
  
  
  * Parameter: `X-Content-Type-Options`
  
  
  
  
Instances: 34
  
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
