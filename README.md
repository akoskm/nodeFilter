nodeFilter is a tiny little jQuery plugin which helps you to write selectors for XML elements, even for those with namespaces.

Usage:


```html
    <prefix:tag color="red" taste="tasty">Apple</prefix:tag>
    <prefix:tag color="green" taste="tasty">Kiwi</prefix:tag>
```

```javascript

    var xmlDoc = $.parseXML(rawXml),
        $xml = $(xmlDoc),
        nodeFilterPTAttr = $xml.nodeFilter('prefix:tag[color="green"]').text(); // Kiwi

```

Tested on Firefox (23.0) and Chrome (29.0.1547.65)
