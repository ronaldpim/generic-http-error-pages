# generic-http-error-pages
Single Page HTTP Error Pages.  These are simple pages that are standalone pages to be either hosted on webserver or off-network (AWS S3) when using AWS-ELB/ALB or AWS-Cloudfront.

##Example

###Nginx Self Hosted
```shell
  error_page 400 /400.html;
  error_page 401 /401.html;
  error_page 403 /403.html;
  error_page 404 /404.html;
  error_page 405 /405.html;
  error_page 406 /406.html;
  error_page 408 /407.html;
  error_page 409 /409.html;
  error_page 410 /410.html;
  error_page 413 /413.html;
  error_page 415 /415.html;
  error_page 417 /417.html;
  error_page 426 /426.html;
  error_page 500 501 502 503 504 505 /500.html;
  location /400.html { root /usr/share/nginx/html; internal; }
  location /401.html { root /usr/share/nginx/html; internal; }
  location /403.html { root /usr/share/nginx/html; internal; }
  location /404.html { root /usr/share/nginx/html; internal; }
  location /405.html { root /usr/share/nginx/html; internal; }
  location /406.html { root /usr/share/nginx/html; internal; }
  location /408.html { root /usr/share/nginx/html; internal; }
  location /409.html { root /usr/share/nginx/html; internal; }
  location /410.html { root /usr/share/nginx/html; internal; }
  location /413.html { root /usr/share/nginx/html; internal; }
  location /415.html { root /usr/share/nginx/html; internal; }
  location /417.html { root /usr/share/nginx/html; internal; }
  location /426.html { root /usr/share/nginx/html; internal; }
  location /500.html { root /usr/share/nginx/html; internal; }
```

## Reference:
[Hypertext Transfer Protocol -- HTTP/1.1 - Section 10](https://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html)
