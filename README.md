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

### Set cookie by name  
```
setCookie(cookieName: string, value: string, validity?: number | Date, domain?: string, path?: string, needsSecureConnection?: boolean)
```

### Delete a cookie by name  
```
deleteCookie(cookieName: string, domain?: string, path?: string)
```

### Check if a cookie exists  
```
exists(cookieName: string): boolean
```
