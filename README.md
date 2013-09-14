nodeFilter is a tiny little jQuery plugin which helps you to write selectors for you XML elements, even for those with namespaces.

Usage

```javascript

    var xmlDoc = $.parseXML(rawXml),
        $xml = $(xmlDoc),
        nodeFilterPTAttr = $xml.nodeFilter('prefix:tag[color="green"]').text();

```