Jonnitto.Picture Package for Neos CMS
=====================================

[![Latest Stable Version](https://poser.pugx.org/jonnitto/picture/v/stable)](https://packagist.org/packages/jonnitto/picture)
[![Total Downloads](https://poser.pugx.org/jonnitto/picture/downloads)](https://packagist.org/packages/jonnitto/picture)
[![License](https://poser.pugx.org/jonnitto/picture/license)](https://packagist.org/packages/jonnitto/picture)

With this package you add a `<picture>` NodeType into [Neos CMS](https://www.neos.io).  
Contributions are very welcome!

Lightbox support
----------------

If you want to add lightbox support you can set the super types on the `Picture` node type:

```
'Jonnitto.Picture:Picture':
  superTypes:
    'Jonnitto.Picture:Lightbox': true
    'Jonnitto.Picture:Caption': true
```

After that, you can install [Jonnitto.PhotoSwipe](https://github.com/jonnitto/Jonnitto.PhotoSwipe) via composer: `composer require jonnitto/photoswipe`  
Et voilà: You've just included [PhotoSwipe](http://photoswipe.com/)



License
-------
The MIT License (MIT)

Copyright (c) 2017 Jon Uhlmann

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
