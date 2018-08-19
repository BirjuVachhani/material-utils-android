# material-utils-android
Library for using material colors in your andorid project

## Benefits
* All material colors are available as color resources
* Contains parsed material colors to use it java files directly. No need to call 'getColor()' to get the color

## Gradle Dependency

* Add the JitPack repository to your project's build.gradle file

```
allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}
```

* Add the dependency in your app's build.gradle file

```
dependencies {
    implementation 'com.github.BirjuVachhani:material-utils-android:1.0.0'
}
```

## Usage

#### XML
```
android:background="@color/material_red_500"
```

### For Theming
```
<style name="AppTheme" parent="Theme.AppCompat.Light.DarkActionBar">
        <!-- Customize your theme here. -->
        <item name="colorPrimary">@color/material_blue_primary</item>
        <item name="colorPrimaryDark">@color/material_blue_primary_dark</item>
        <item name="colorAccent">@color/material_pink_accent</item>
    </style>
```

### Java
```
//No need to parse colors, just use library's materialColor class
textView.setTextColor(MaterialColor.RED_500)
textView.setBackgroundColor(MaterialColor.YELLOW_500)
```

## Licence

&copy; 2018 Birju Vachhani

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
