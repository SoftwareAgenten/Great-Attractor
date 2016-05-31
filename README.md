# Great-Attractor

## Usage

Include the following snippet in the PHP file that you want to track. Naming your pages with `ga_init($page_name)` helps you filter for individual pages using the [GA-Analyzer](https://github.com/SoftwareAgenten/GA-Analyzer).

```php
<?php

# GA

include_once('great−attractor/system.php');

ga_init('tracking−name');
ga_register_visit();
ga_register_request();

if (!empty($_POST)) {
  ga_register_form_data_($_POST);
}

# END GA
```