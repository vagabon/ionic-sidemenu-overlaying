# Ionic SideMenu Overlaying

This is an angular's directive for ionic 1.1.0, the sidemenu will expand all over the main content.

Demo :

## Install

Load the js with requireJs :

 * Include in the PATH
 
```JAVASCRIPT
    require.config({
        paths: {
        ...
        "ionic-sidemenu-overlaying": '../lib/ionic-sidemenu-overlaying/dist/ionic-sidemenu-overlaying',
        ...
```

 * Add it to the project

```JAVASCRIPT
    require([
        'ionic',
        'ionic-sidemenu-overlaying',
    ], function () {
        ...
```

 * Load the Angular Module in your App

```JAVASCRIPT
    angular.module('<your_main_angular_module>', ['ionic', 'ionic-sidemenu-overlaying', ...])
```

 * HTML

```HTML
    <ion-side-menus>
        <ion-side-menu-content>
            <ion-nav-bar class="bar-stable">
                <ion-nav-buttons side="left">
                    <button class="button button-icon button-clear ion-navicon" menu-toggle="left"></button>
                </ion-nav-buttons>
            </ion-nav-bar>
            <ion-nav-view name="menuContent" drag-content="false"></ion-nav-view>
        </ion-side-menu-content>

        <ion-side-menu side="left" edge-drag-threshold="200">
            <ion-content>
                <ion-list>...</ion-list>
            </ion-content>
        </ion-side-menu>
    </ion-side-menus>
```

## Integration in bower

```JAVASCRIPT
    "dependencies": {
        ...
        "ionic-sidemenu-overlaying": "vagabon/ionic-sidemenu-overlaying#>=1.0.0",
        ...
```

 * Update the libs of your project

```SHELL
    #bower update
```

