# rocket-dark

##Usage

Advanced -> Custom code

```
function applycss(css) {
    var head = document.getElementsByTagName('head')[0];
    var s = document.createElement('style');
    s.setAttribute('type', 'text/css');
    s.appendChild(document.createTextNode(css));
    head.appendChild(s);
}

fetch('https://api.github.com/repos/rukuh/rocket-dark/contents/dark.css').then(res => res.json()).then(css => applycss(window.atob(css.content)));
```
