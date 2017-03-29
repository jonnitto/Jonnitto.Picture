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

Licensed under MIT, see [LICENSE](LICENSE)
