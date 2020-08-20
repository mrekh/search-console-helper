# Search Console Helper - Show performance report

A simple bookmarklet that adds the current browser URL to your clipboard, and opens Perfomacne report of that URL (Exact URL) in Search Console for that property.

All you need to do is paste straight into the URL inspection bar.


## Bookmarklet

Copy and paste the code below into a bookmark.
```
javascript:(function(){let pathname2 = encodeURI(window.location.pathname);if (window.location.pathname !== pathname2) {window.open("https://search.google.com/search-console/performance/search-analytics?resource_id="+window.location.origin+"&page=!"+window.location.origin+encodeURI(window.location.pathname).toUpperCase());} else {window.open("https://search.google.com/search-console/performance/search-analytics?resource_id="+window.location.origin+"&page=!"+window.location.origin+window.location.pathname);}})();
```

