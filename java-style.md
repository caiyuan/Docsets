
## stylesheet.css

```css
/**===================================================================================**/

pre, code, tt {
  font-family: 'Fira Code', 'DejaVu Sans Mono', monospace;
  color: #4CAF50;
}

a * {
  color: #03a9f4;
}

a:link, a:visited {
  color: #03a9f4;
}
```

## jquery.js

```javascript
// ===============================================

$(function() {
	var lang = "";
	var r = window.location.href;
	if(r.search("/en/") == -1) {
		lang = r.replace(/\/api\//i,"/api/en/");
	} else {
		lang = r.replace(/\/api\/en\//i,"/api/");
	}
    $("header .topNav .navList").append("<li><a href=\""+lang+"\">中文 & 英文</a></li> ");
});
```

