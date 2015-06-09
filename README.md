ToggleButton
============

ToggleButton Widget For Android Developers

<img src="https://github.com/Tinker-S/ToggleButton/blob/master/toggle.gif"/>

## Status

This plugin has already published to **jCenter**, but not on Maven Central yet.  

* [jCenter](https://bintray.com/tinker-s/maven/ToggleButton)

## Usage

To use this plugin, you need add some code in your **build.gradle**:

* Ensure you have included jcenter repository

```
repositories {
    jcenter()
}
```

* Add dependencies

```
compile 'com.awesomego.togglebutton:library:1.0.0'
```

* Use in your layout

```
xmlns:toggle="http://schemas.android.com/apk/res-auto"
```

```
<com.awesomego.widget.ToggleButton
    android:layout_width="54dp"
    toggle:onColor="#f00"
    toggle:offColor="#ddd"
    toggle:spotColor="#00f"
    toggle:offBorderColor="#000"
    toggle:borderWidth="2dp"
    android:layout_height="30dp" />
```

* Use in your java code

```
ToggleButton toggleBtn;
        
//切换开关
toggleBtn.toggle();
//切换无动画
toggleBtn.toggle(false);
//开关切换事件
toggleBtn.setOnToggleChanged(new OnToggleChanged(){
    @Override
    public void onToggle(boolean on) {
    }
});
        
toggleBtn.setToggleOn();
toggleBtn.setToggleOff();
//无动画切换
toggleBtn.setToggleOn(false);
toggleBtn.setToggleOff(false);

//禁用动画
toggleBtn.setAnimate(false);
```

## Attention

If you have found any bugs or need some features, please create an issue at [Github Issue Tracker](https://github.com/Tinker-S/ToggleButton/issues).

## License

    Copyright (C) 2015 Tinker Sun

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.