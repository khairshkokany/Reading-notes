## THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS


### DIVING IN
**ersistent local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.**

### three potentially dealbreaking downsides:

1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.
2.Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL).
3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.


### What we really want is


1. a lot of storage space
2. on the client
3. that persists beyond a page refresh
4. and isn’t transmitted to the server


## A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5


**In the beginning, there was only Internet Explorer. Or at least, that’s what Microsoft wanted the world to think. To that end, as part of the First Great Browser Wars, Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer. One of these things was called DHTML Behaviors, and one of these behaviors was called userData.**

**userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. (Trusted domains, such as intranet sites, can store 10 times that amount. And hey, 640 KB ought to be enough for anybody.) IE does not present any form of permissions dialog, and there is no allowance for increasing the amount of storage available.**


## HTML5 STORAGE SUPPORT 
IE	FIREFOX	SAFARI	CHROME	OPERA	IPHONE	ANDROID
8.0+	3.5+ 	4.0+   	4.0+  	10.5+	 2.0+   	2.0+

**From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object. Before you can use it, you should detect whether the browser supports it.**

> Example 

function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}

## USING HTML5 STORAGE

**HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.**

> Example

interface Storage {
  getter any getItem(in DOMString key);
  setter creator void setItem(in DOMString key, in any data);
};


## LIMITATIONS IN CURRENT BROWSERS

**In talking about the history of local storage hacks using third-party plugins, I made a point of mentioning the limitations of each technique, such as storage limits. I just realized that I haven’t mentioned anything about the limitations of the now-standardized HTML5 Storage. I’ll give you the answers first, then explain them. The answers, in order of importance, are “5 megabytes,” “QUOTA_EXCEEDED_ERR,” and “no.”**

## HTML5 STORAGE IN ACTION

### How does it work? Every time a change occurs within the game, we call this function:

function saveGameState() {
    if (!supportsLocalStorage()) { return false; }
    localStorage["halma.game.in.progress"] = gGameInProgress;
    for (var i = 0; i < kNumPieces; i++) {
	localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
	localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
    }
    localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
    localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
    localStorage["halma.movecount"] = gMoveCount;
    return true;
}


## BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS


>  actual working code in 4 browsers


openDatabase('documents', '1.0', 'Local document storage', 5*1024*1024, function (db) {
  db.changeVersion('', '1.0', function (t) {
    t.executeSql('CREATE TABLE docids (id, name)');
  }, error);
});



