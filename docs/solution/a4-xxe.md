# XML External Entities

## XXE in XYZ

There is a SQL Injection in `User Search` feature at the following URL  

http://127.0.0.1:9090/app/usersearch

**Vulnerable Code snippet**

*core/appHandler.js*
```         
...

...
```
**Solution**


*core/appHandler.js*
```
...

...
```

But it is recommended to explicitly validate/sanitize inputs

**Fixes**

Implemented in the following files

- *core/appHandler.js*

**Recommendation**

- Validate Input before processing
- Sanitize Input before storing

**Reference**

- <https://www.owasp.org/index.php/Top_10-2017_A4-XML_External_Entities_(XXE)>