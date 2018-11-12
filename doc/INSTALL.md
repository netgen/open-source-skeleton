Installation instructions
=========================

Requirements
------------

* eZ Platform 2.0+

Installation steps
------------------

### Use Composer

Run the following from your website root folder to install the package:

```bash
$ composer require netgen/my-demo-bundle
```

### Activate the bundle

Activate required bundles in `app/AppKernel.php` file by adding them to the `$bundles` array in `registerBundles` method:

```php
public function registerBundles()
{
    ...
    $bundles[] = new Netgen\Bundle\MyExampleBundle\NetgenMyExampleBundle();

    return $bundles;
}
```
 

### Clear the caches

Clear the eZ Platform caches with the following command:

```bash
$ php bin/console cache:clear
```

For more detailed configuration, please check [documentation](DOC.md).