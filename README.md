# Spring Session Concurrency Test
Steps to reproduce are:
* Run redis localhost at default port with config:

```
    config set notify-keyspace-events KEA
    config get notify-keyspace-events
```

* Standard Spring Boot 2 Application with Maven, So run 
    class FacebookLoginApplication with main
    method(I was using Java 11 on my machine).

* Just provide oauth2-filter.properties in resources folder
  to provider OAuth Providers credentials(Using maven resource
  filtering) in given template:
 ```
 google.client-id=Your Client Id
 google.client-secret=Your Client Secret
 facebook.client-id=Your Client Id
 facebook.client-secret=Your Client Secret
 linkedin.client-id=Your Client Id
 linkedin.client-secret=Your Client Secret
 ```

