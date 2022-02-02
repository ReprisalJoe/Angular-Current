# Project - Angular-Current

## Visual Studio 2022 .Net Angular 5 project, with HTTPS configure option.
### Changes
It has been upgraded to a clean **Angular 13.2.0**
As of Version 2.0 ng-connection-service has been removed until it can be fixed

With templating variables added you must use the release or download this and save it as a template.
It will not work unless you export as a template.

~~It will compile and run cleanly on fork.~~
It has been modified

WeatherController removed
~~Controllers\WeatherForecastControll.cs


~~ClientApp\src\app\counter~~
~~ClientApp\src\app\fetch-data~~

Changes to
ClientApp\src\app\Nav-menu.component.html
The following code is removed

```
<li class="nav-item" [routerLinkActive]="['link-active']">
  <a class="nav-link text-dark" [routerLink]="['/counter']"
    >Counter</a
  >
</li>
<li class="nav-item" [routerLinkActive]="['link-active']">
  <a class="nav-link text-dark" [routerLink]="['/fetch-data']"
    >Fetch data</a
  >
</li>
```

It has cache-control added in appsettings.json. 
```
  "StaticFiles": {
    "Headers": {
      "Cache-Control": "max-age=3600"
    }
  }
````
Angular routing has been moved to a dedicated typescript module -> app-routing.module.ts
