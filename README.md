Navegador
=========

Navegador Creado sin Fines de Luco
<? xml version = " 1.0 " codificación = " UTF-8 " ?>
<! -
  Derechos de Autor 2014 Desarrollo ACR
->

< manifiestos  xmlns : android = " http://schemas.android.com/apk/res/android "
    paquete = " acr.browser.lightning "
    Android : versionCode = " 66 "
    Android : VersionName = " 3.2.0.1a " >

    < usa-permiso  androide : nombre = " android.permission.INTERNET " />
    < usa-permiso  androide : nombre = " com.android.browser.permission.READ_HISTORY_BOOKMARKS " />
    < usa-permiso  androide : nombre = " com.android.browser.permission.WRITE_HISTORY_BOOKMARKS " />
    < usa-permiso  androide : nombre = " android.permission.WRITE_EXTERNAL_STORAGE " />
    < usa-permiso  androide : nombre = " android.permission.READ_EXTERNAL_STORAGE " />
    < usa-permiso  androide : nombre = " android.permission.ACCESS_FINE_LOCATION " />
    < usa-permiso  androide : nombre = " android.permission.ACCESS_NETWORK_STATE " />

    < usos-feature
        android : name = " android.hardware.location.gps "
        Android : requerido = " false " />
    < usos-feature
        Android : nombre = " android.hardware.location "
        Android : requerido = " false " />
    < usos-feature
        android : name = " android.hardware.touchscreen "
        Android : requerido = " false " />

    < usos-sdk
        Android : minSdkVersion = " 14 "
        Android : targetSdkVersion = " 20 " />

    < aplicación
        Android : nombre = " acr.browser.lightning.BrowserApp "
        Android : allowBackup = " verdadera "
        Android : hardwareAccelerated = " verdadera "
        android : icon = " @ estirable / ic_launcher "
        android : label = " @ string / nombre_apl " >
        < actividad
            Android : nombre = " acr.browser.lightning.MainActivity "
            Android : alwaysRetainTaskState = " verdadera "
            Android : configChanges = " orientación | ScreenSize | keyboardHidden | Teclado "
            android : label = " @ string / nombre_apl "
            Android : launchMode = " singleTask "
            Android : tema = " @ style / LightTheme " >
            < intención de filtro >
                < acción  androide : nombre = " android.intent.action.MAIN " />

                < categoría  androide : nombre = " android.intent.category.DEFAULT " />
                < categoría  androide : nombre = " android.intent.category.LAUNCHER " />
                < categoría  androide : nombre = " android.intent.category.BROWSABLE " />
                < categoría  androide : nombre = " android.intent.category.APP_BROWSER " />
            </ intención de filtro >
            < intención de filtro >
                < acción  androide : nombre = " android.intent.action.VIEW " />

                < categoría  androide : nombre = " android.intent.category.DEFAULT " />
                < categoría  androide : nombre = " android.intent.category.BROWSABLE " />

                < datos  androide : esquema = " http " />
                < datos  androide : esquema = " https " />
                < datos  androide : esquema = " acerca " />
                < datos  androide : esquema = " javascript " />
            </ intención de filtro >
            <! -
                  Para estos planes en los que cualquiera de estos tipos MIME particulares
                  se han suministrado, somos un buen candidato.
            ->
            < intención de filtro >
                < acción  androide : nombre = " android.intent.action.VIEW " />

                < categoría  androide : nombre = " android.intent.category.BROWSABLE " />
                < categoría  androide : nombre = " android.intent.category.DEFAULT " />

                < datos  androide : esquema = " http " />
                < datos  androide : esquema = " https " />
                < datos  androide : esquema = " inline " />
                < datos  androide : mimeType = " text / html " />
                < datos  androide : mimeType = " text / plain " />
                < datos  androide : mimeType = " application / xhtml + xml " />
                < datos  androide : mimeType = " application / vnd.wap.xhtml + xml " />
            </ intención de filtro >
            <! - Para ver archivos web guardadas. ->
            < intención de filtro >
                < acción  androide : nombre = " android.intent.action.VIEW " />

                < categoría  androide : nombre = " android.intent.category.BROWSABLE " />
                < categoría  androide : nombre = " android.intent.category.DEFAULT " />

                < datos  androide : esquema = " http " />
                < datos  androide : esquema = " https " />
                < datos  androide : esquema = " archivo " />
                < datos  androide : mimeType = " application / x-webarchive-xml " />
            </ intención de filtro >
            < intención de filtro >
                < acción  androide : nombre = " android.intent.action.WEB_SEARCH " />

                < categoría  androide : nombre = " android.intent.category.DEFAULT " />
                < categoría  androide : nombre = " android.intent.category.BROWSABLE " />

                < datos  androide : esquema = " " />
                < datos  androide : esquema = " http " />
                < datos  androide : esquema = " https " />
            </ intención de filtro >
        </ actividad >
        < actividad
            Android : nombre = " acr.browser.lightning.SettingsActivity "
            Android : configChanges = " orientación | ScreenSize | keyboardHidden | Teclado "
            Android : etiqueta = " @ string / ajustes "
            Android : tema = " @ style / DefaultTheme " >
            < intención de filtro >
                < acción  androide : nombre = " android.intent.action.SETTINGS " />

                < categoría  androide : nombre = " android.intent.category.DEFAULT " />
            </ intención de filtro >
        </ actividad >
        < actividad
            Android : nombre = " acr.browser.lightning.AdvancedSettingsActivity "
            Android : configChanges = " orientación | ScreenSize | keyboardHidden | Teclado "
            android : label = " @ string / avanzado "
            Android : tema = " @ style / DefaultTheme " >
            < intención de filtro >
                < acción  androide : nombre = " android.intent.action.ADVANCED_SETTINGS " />

                < categoría  androide : nombre = " android.intent.category.DEFAULT " />
            </ intención de filtro >
        </ actividad >
        < actividad
            Android : nombre = " acr.browser.lightning.IncognitoActivity "
            Android : alwaysRetainTaskState = " verdadera "
            Android : configChanges = " orientación | ScreenSize | keyboardHidden | Teclado "
            android : label = " @ string / nombre_apl "
            Android : launchMode = " singleTask "
            Android : tema = " @ style / DarkTheme "
            Android : windowSoftInputMode = " stateHidden " >
            < intención de filtro >
                < acción  androide : nombre = " android.intent.action.INCOGNITO " />

                < categoría  androide : nombre = " android.intent.category.DEFAULT " />
            </ intención de filtro >
        </ actividad >
        < actividad
            Android : nombre = " acr.browser.lightning.LicenseActivity "
            Android : configChanges = " orientación | ScreenSize | keyboardHidden | Teclado "
            Android : etiqueta = " @ string / licencias "
            Android : tema = " @ style / DefaultTheme " >
            < intención de filtro >
                < acción  androide : nombre = " android.intent.action.LICENSE " />

                < categoría  androide : nombre = " android.intent.category.DEFAULT " />
            </ intención de filtro >
        </ actividad >
        
        < actividad
            Android : nombre = " acr.browser.lightning.BookmarkActivity "
            Android : configChanges = " orientación | ScreenSize | keyboardHidden | Teclado "
            Android : etiqueta = " @ string / bookmark_settings "
            Android : tema = " @ style / DefaultTheme " >
            < intención de filtro >
                < acción  androide : nombre = " android.intent.action.BOOKMARK " />

                < categoría  androide : nombre = " android.intent.category.DEFAULT " />
            </ intención de filtro >
        </ actividad >
    </ aplicación >

</ manifiesto >
