# Search Console Helper

A simple bookmarklet that adds the current browser URL to your clipboard, and opens Perfomacne report of that URL (Exact URL) in Search Console for that property.

All you need to do is paste straight into the URL inspection bar.


## Bookmarklet

Copy and paste the code below into a bookmark.
```javascriptjavascript:(function(){let mrekh=document.createElement("textarea");document.body.appendChild(mrekh),mrekh.value=window.location.href,mrekh.select(),document.execCommand("copy"),document.body.removeChild(mrekh),window.open("https://search.google.com/search-console/performance/search-analytics?resource_id="+window.location.origin+"&page=!"+window.location.href)})();
```

