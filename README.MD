


### Installation

```composer require nadsoft/breads-seed```


```
1- write this command (php artisan vendor:publish --provider="DrudgeRajen\VoyagerDeploymentOrchestrator\VoyagerDeploymentOrchestratorServiceProvider") 
```
```
2- go to path  `config/voyager-deployment-orchestrator.php` and add the tables name of which BREAD seeders will be generated , each table you will used in bread you must add it in this array
```
for example ..
```
return [
    'tables' => [
        "projects"
    ],
];
```

After Publishing the `VoyagerDeploymentOrchestratorSeeder` class file,
autoload composer so that laravel knows about new seeders.

``composer dump-autoload``

### Usage
```
3- go to path (```database/Seeders/VoyagerDeploymentOrchestratorSeeder```) and 
add this namespace ("namespace Database\Seeders;") and each bread created you must import it in this file;

```
### To run the seeder file:
```
4- to run seeder you must write this command (```php artisan db:seed --class=VoyagerDeploymentOrchestratorSeeder```)
```

###
Develop By <a href="https://github.com/DrudgeRajen/"> DrudgeRajen </a> 

Updated By  <a href="https://nadsoft.net/"> Nadsoft Company </a>
