


### Installation

```composer require drudge-rajen/voyager-deployment-orchestrator:dev-master```

1- download this package above of page from github  and replace it in this path (vendor\drudge-rajen\voyager-deployment-orchestrator)



```
2- write this command (php artisan vendor:publish --provider="DrudgeRajen\VoyagerDeploymentOrchestrator\VoyagerDeploymentOrchestratorServiceProvider") 
```

3- go to path  `config/voyager-deployment-orchestrator.php` and add the tables name of which BREAD seeders will be generated , each table you will used in bread you must add it in this array

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

4- go to path (```database/Seeders/VoyagerDeploymentOrchestratorSeeder```) and add this namespace ("namespace Database\Seeders;") and each bread created you must import it in this file;


### To run the seeder file:

5- to run seeder you must write this command (```php artisan db:seed --class=VoyagerDeploymentOrchestratorSeeder```)


###
Develop By <a href="https://github.com/DrudgeRajen/"> DrudgeRajen </a> 

```Redevelop By  Nadsoft Company ```
