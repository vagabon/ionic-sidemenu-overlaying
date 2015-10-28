# Ionic SideMenu Overlaying

This is an angular's directive for ionic 1.1.0, the sidemenu will expand all over the main content.

Demo :

## Install

Load the js with requireJs :

 * Include in the PATH

    require.config({
        paths: {
            ...
            "ionic-slidemenu-overlaying": '../lib/ionic-slidemenu-overlaying/dist/ionic-slidemenu-overlaying',
            ...

 * Add it to the project

    require([
      'ionic',
      'ionic-slidemenu-overlaying'
    ], function () {
        ...

 * Load the Angular Module in your App

    angular.module('<your_main_angular_module>', ['ionic', 'ionic-slidemenu-overlaying', ...])

 * HTML

    <ion-side-menus>
      <ion-side-menu-content>
        <ion-nav-bar class="bar-stable">

          <ion-nav-buttons side="left">
            <button class="button button-icon button-clear ion-navicon" menu-toggle="left">
            </button>
          </ion-nav-buttons>
        </ion-nav-bar>

        <ion-nav-view name="menuContent" drag-content="false"></ion-nav-view>
      </ion-side-menu-content>

      <ion-side-menu side="left" edge-drag-threshold="200">
        <ion-content>
          <ion-list>
            ...
          </ion-list>
        </ion-content>
      </ion-side-menu>
    </ion-side-menus>

## Integration in bower


  "dependencies": {
    ...
    "ionic-sidemenu-overlaying": "vagabon/ionic-sidemenu-overlaying#>=1.0.0",
    ...


    ```shell
    bower update
    ```

