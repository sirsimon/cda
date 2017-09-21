# Snippets

### CDA movie

```javascript
var a = $('.brdPlayerWrapper object [name=flashvars]').attr('value');
var b = a.substring($('.brdPlayerWrapper object [name=flashvars]').attr('value').indexOf('file=') + 5);
    b = decodeURIComponent(b.substring(0, b.indexOf('&')));
```

### Redmine log

```javascript
var b = [], a = [];
$($0).parents('dl').find('a').each(function() {
    if ($(this)[0].text.indexOf('#') > -1) {
    	var id = $(this)[0].text.match(/#\d+/)[0];
        if (b.indexOf(id) === -1) {
            a.push(id + ' ' + $(this)[0].text.match(/: .*/)[0].substr(2));
            b.push(id);
        }
    }
});
"\n" + a.reverse().join("\n") + "\n";
```