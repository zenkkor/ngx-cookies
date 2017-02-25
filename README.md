# ngx-cookies
A simple cookies package for Angular X (Angular 2+).  

# How to install?  

`$ npm install ngx-cookies`   

```
import { NgXCookies } from 'ngx-cookies';
```  

Use static methods as pleased.  

## Available methods

### Get cookie by name  
```
getCookie(cookieName: string): string
```

Example: `NgXCookies.getCookie(<ID>);`  


### Set cookie by name  

Default validityType is in minutes. Also accepts hours || days

```
setCookie(cookieName: string, value: string, validity?: number, validityType?: string, domain?: string, path?: string, needsSecureConnection?: boolean)
```

Example cookie that expires in 24hrs: `NgXCookies.setCookie(<ID>, <VALUE>, 24, 'hours');`  

### Delete a cookie by name  
```
deleteCookie(cookieName: string, domain?: string, path?: string)
```

Example: `NgXCookies.deleteCookie(<ID>);`  


### Check if a cookie exists  
```
exists(cookieName: string): boolean
```

Example: `NgXCookies.exists(<ID>);`  
