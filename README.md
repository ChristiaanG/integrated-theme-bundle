# IntegratedThemeBundle #
This bundle provides theme support

## Requirements ##
* See the require section in the composer.json

## Features ##
* Theme support

## Documentation ##
* [Integrated for Developers](http://integratedfordevelopers.com/ "Integrated for Developers")

## Installation ##
This bundle can be installed following these steps:

### Install using composer ###

    $ php composer.phar require integrated/theme-bundle:~0.3

### Enable the bundle ###

    // app/AppKernel.php
    public function registerBundles()
    {
        return array(
            // ...
            new Integrated\Bundle\ThemeBundle\IntegratedThemeBundle()
            // ...
        );
    }

### Configuration ###

    # app/config/config.yml
    integrated_theme:
        themes:
            mytheme1:
                paths: 
                    - @AppBundle/Resources/views/themes/mytheme1
                fallback: 
                    - default
            mytheme2:
                paths:
                    - @AppBundle/Resources/views/themes/mytheme2
                    - @OtherBundle/Resources/views/themes/mytheme2
                fallback: 
                    - mytheme1
                    - mytheme3

## License ##
This bundle is under the MIT license. See the complete license in the bundle:

    LICENSE

## Contributing ##
Pull requests are welcome. Please see our [CONTRIBUTING guide](http://integratedfordevelopers.com/contributing "CONTRIBUTING guide").

## About ##
This bundle is part of the Integrated project. You can read more about this project on the
[Integrated for Developers](http://integratedfordevelopers.com/ "Integrated for Developers") website.
