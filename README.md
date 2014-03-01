# PreensterWeb


## Instalizing
To install, insert the following code on the page before closing «body» tag: 

``` js
 	var _preensterConfig = _preensterConfig || {};
	_preensterConfig.scriptsPath = 'http://web.preenster.com/script';
	_preensterConfig.host = document.location.hostname;

	(function() {
          var ps = document.createElement('script'); ps.type = 'text/javascript'; ps.async = true;
	  ps.src =  _preensterConfig.scriptsPath + '/insert.js';
	  var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ps, s);
	})();
```

For example:
``` html
<html>
    <head>
        <title></title>
    </head>
<body>


## site content ##


<script>
 	var _preensterConfig = _preensterConfig || {};
	_preensterConfig.scriptsPath = 'http://web.preenster.com/script';
	_preensterConfig.host = document.location.hostname;

	(function() {
          var ps = document.createElement('script'); ps.type = 'text/javascript'; ps.async = true;
	  ps.src =  _preensterConfig.scriptsPath + '/insert.js';
	  var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ps, s);
	})();
</script>
</body>
</html>
```
