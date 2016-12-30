# EzLandigPageLayoutsBundle
 
This bundle will add some layouts (see screenshot in doc folder) to the standard Landingpage. Each of this layouts is using one or more zones. The content of the landingpage will be added later as blocks in the different zones.
 
 ## Prerequisites
 * **eZ Platform Enterprise Edition (clean installation)**
 * bootstrap framework   (you have to change the layouts template if you are using other framework)
 
 Tested with Ez Platform Enterprise Edition 1.7.0 LTS (clean installation)
 
 ## Features
 * New Layouts in clean eZ Platform Enterprise Edition installation to select during creating new landingpages
 * Quickly re-use this out-of-the-box bundle in different projects
 * Using the same logic to add new layouts
 * Responsive design for every devices
 

## Installation
Clone or download the bundle in your src folder

Then add it to your application:

```php
// app/AppKernel.php

    public function registerBundles()
    {   
        $bundles = array(  
        // ...
        new EzLandigPageLayoutsBundle\EzLandigPageLayoutsBundle(),
        // ...
    );
}
```


The landing_page full template is located in:
```
    src/EzLandigPageLayoutsBundle/Resources/views/full/landing_page.html.twig
```
Change the first line with your root or base Template location. More on how to create root Template can be found here [Content rendering configuration](https://doc.ez.no/display/DEVELOPER/Step+3+-+Customizing+the+general+layout)

Create assets
```
php app/console assets:install --symlink
```

Clear cache (production add : --env=prod)
```
php app/console cache:clear
```
