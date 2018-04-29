[![Latest Stable Version](https://poser.pugx.org/jonnitto/picture/v/stable)](https://packagist.org/packages/jonnitto/picture)
[![Total Downloads](https://poser.pugx.org/jonnitto/picture/downloads)](https://packagist.org/packages/jonnitto/picture)
[![License](https://poser.pugx.org/jonnitto/picture/license)](LICENSE)
[![GitHub forks](https://img.shields.io/github/forks/jonnitto/Jonnitto.Picture.svg?style=social&label=Fork)](https://github.com/jonnitto/Jonnitto.Picture/fork)
[![GitHub stars](https://img.shields.io/github/stars/jonnitto/Jonnitto.Picture.svg?style=social&label=Stars)](https://github.com/jonnitto/Jonnitto.Picture/stargazers)
[![GitHub watchers](https://img.shields.io/github/watchers/jonnitto/Jonnitto.Picture.svg?style=social&label=Watch)](https://github.com/jonnitto/Jonnitto.Picture/subscription)
[![GitHub followers](https://img.shields.io/github/followers/jonnitto.svg?style=social&label=Follow)](https://github.com/jonnitto/followers)
[![Follow Jon on Twitter](https://img.shields.io/twitter/follow/jonnitto.svg?style=social&label=Follow)](https://twitter.com/jonnitto)

# Jonnitto.Picture Package for Neos CMS

With this package you add a `<picture>` NodeType into [Neos CMS](https://www.neos.io).  
Contributions are very welcome!

## Installation

Most of the time you have to make small adjustments to a package (e.g. configuration in Settings.yaml). Because of that, it is important to add the corresponding package to the composer from your theme package. Mostly this is the site packages located under Packages/Sites/. To install it correctly go to your theme package (e.g.Packages/Sites/Foo.Bar) and run following command:

```bash
composer require jonnitto/picture --no-update
```

The --no-update command prevent the automatic update of the dependencies. After the package was added to your theme composer.json, go back to the root of the Neos installation and run composer update. Et voilà! Your desired package is now installed correctly.

## Lightbox support

If you want to add lightbox support you can set the super types on the `Picture` node type:

```yaml
'Jonnitto.Picture:Picture':
  superTypes:
    'Jonnitto.Picture:Lightbox': true
    'Jonnitto.Picture:Caption': true
```

After that, you can install [Jonnitto.PhotoSwipe](https://github.com/jonnitto/Jonnitto.PhotoSwipe) via composer: `composer require jonnitto/photoswipe`  
Et voilà: You've just included [PhotoSwipe](http://photoswipe.com/)

## License

Licensed under MIT, see [LICENSE](LICENSE)
