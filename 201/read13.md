# ***Read: 13 - Local Storage***
- - - 
## The Past, Present, and Future of Local Storage for Web Applications

### before html5 

***Cookies*** can be used for persistent local storage of small amounts of data. But they have some dealbreaking downsides:
Cookies are included with every HTTP request, thereby sending data unencrypted over the internet and Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.

* What needed is : a lot of storage space, on the client ,that persists beyond a page refresh and isn’t transmitted to the server .

* ***userData*** allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure.(Trusted domains,can store 10 times that amount )
no permissions dialog no allowance for increasing the amount of storage available.
* In 2002, Adobe introduced a feature in Flash 6 “Flash cookies” this feature is properly known as Local Shared Objects. store up to 100 KB of data per domain.    

 all of the soulutions are either specific to a single browser, or reliant on a third-party plugin. 

### HTML5 STORAGE ( Web Storage)

Certain browser vendors also refer to it as “Local Storage” or “DOM Storage    

> it’s a way for web pages to store named key/value pairs locally, within the client web browser.   

this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server    

From JavaScript code, we can access HTML5 Storage through the localStorage object on the global window object.     
function supports_html5_storage() {     
  try {    
    return 'localStorage' in window && window['localStorage'] !== null;    
  } catch (e) {   
    return false;   
  }   
}   
or Instead of writing this function yourself, you can use Modernizr to detect support for HTML5 Storage.

#### USING HTML5 STORAGE

* HTML5 Storage is based on named key/value pairs   
* You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript   
* the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

#### TRACKING CHANGES TO THE HTML5 STORAGE AREA

* If you want to keep track programmatically of when the storage area changes, you can trap the storage event
* The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.
* The storage event is supported everywhere the localStorage object is supported


