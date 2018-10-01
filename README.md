# external-links-new-tab
Open External Links in a New Tab (jQuery - Kevin's Code)

```
jQuery('a').map(function (i, el) {
    var elem = $(el);
    var href = elem.attr('href');
    var host = window.location.host;
    if (href.indexOf(host) < 0 && href.indexOf('http') > -1) {
        elem.attr('target', '_blank');
    }
});
```
