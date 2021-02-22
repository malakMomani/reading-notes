## THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS

- **In the beginning** , there was only Internet Explorer . it was having sth called `userData`

- `userData` : allowsc to store up 64 KB of data per domain 

- **In 2002** : in *Flash* enviroment from *Adobe* was a feature called "Local Shared Objects" , allows to store up to 100 KB of data per domain.

- **By 2006** : from *ExternalInterface* in *flash 8* , Flash gives each domain 100 KB of storage “for free.” Beyond that, it prompts the user for each order of magnitude increase in data storage (1 Mb, 10 Mb, and so on).

- **In 2007** : *Gears* from *Google* , can store unlimited ammount of data per domain.

- **By 2009** : `dojox.storage` could auto-detect these previous hacks.

## INTRODUCING HTML5 STORAGE
- Web storage , Local Storage , DOM Storage
- What is *HTML5 Storage* : it’s a way for web pages to store named key/value pairs locally, within the client web browser. 

- to check HTML5 Storage :

```
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```

- store data and retrieve it :

```
var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);
```

**OR**

```
var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;
```

![Object](pics/read.jpg)