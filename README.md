Jonnitto.Picture Package for Neos CMS
=====================================

[![Latest Stable Version](https://poser.pugx.org/jonnitto/picture/v/stable)](https://packagist.org/packages/jonnitto/picture)
[![Total Downloads](https://poser.pugx.org/jonnitto/picture/downloads)](https://packagist.org/packages/jonnitto/picture)
[![License](https://poser.pugx.org/jonnitto/picture/license)](https://packagist.org/packages/jonnitto/picture)

With this package you add a `<picture>` NodeType into [Neos CMS](https://www.neos.io).  
Contributions are very welcome!

Installation
------------
Most of the time you have to make small adjustments to a package (e.g. configuration in Settings.yaml). Because of that, it is important to add the corresponding package to the composer from your theme package. Mostly this is the site packages located under Packages/Sites/. To install it correctly go to your theme package (e.g.Packages/Sites/Foo.Bar) and run following command:

```
composer require jonnitto/picture --no-update
```

The --no-update command prevent the automatic update of the dependencies. After the package was added to your theme composer.json, go back to the root of the Neos installation and run composer update. Et voilà! Your desired package is now installed correctly.


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
