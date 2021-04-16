# external-links-new-tab
Open External Links in a New Tab

```
[...document.querySelectorAll('a')].map(function (el) {
    let href = el.getAttribute('href'),
        host = window.location.host;
    if (host && href) {
        if (href.indexOf(host) < 0 && href.indexOf('http') > -1) {
            el.setAttribute('target', '_blank');
        }
    }
});
```
