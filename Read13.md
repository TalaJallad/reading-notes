# Local Storage for Web Data

* Before HTML5, windows campe up with userData that allows web pages to store up to 64 KB of data per domain, a huge accomplishment comared to the 4KB cookies stored.
* All the old storages were either specific to a single browser, or reliant on a third-party plugin. 
* HTML5 storage/Local storage/DOM storage provides a standardized API and implements natively and consistently in multiple browsers without having to rely on third-party plugins.
*  HTML5 allows web pages to store named key/value pairs locally within the client web browser.
* HTML5 stores data as strings. To change the data type, we can use functions like `parseInt()` or `parseFloat()`.
* If we call `setItem()` with a named key that already exists will silently overwrite the previous value. 
* If we call `getItem()` with a non-existent key will return null rather than throw an exception.
* We can treat the localStorage object as an associative array, for instance: 

```
var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);
```
The above code can be rewritten to use square bracket syntax:

```
var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;
```
* To remove a key's value or clear the storage: 
 ```
 interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};
```