#HexagonMenu
------

HexagonMenu is an implementation of two designs from Dribbble [Menu Concept (iOS)][1] and [Hexagonal flat menu][2].


## Usage
1.About the position of menu item.
  Check out those coordinates in the following screenshot.
  <img src="https://git.oschina.git/robust/HexagonMenu/screenshot/screenshot_03.png" width="320" height="568" />

2.About gravity.
  The same with TextView unless it can not be top|bottom or left|right. Use match_parent instead.
  example:
```xml
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:hex="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <cn.robust.hexagon.library.menu.HexagonMenu
        android:id="@+id/menu"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        hex:gravity="top|center_horizontal"
        android:background="@color/hexa_bg"
        android:padding="5dp" />

</RelativeLayout>
```

3.For more details, just look at the sample project.


  [1]: https://dribbble.com/shots/1193991-Menu-Concept-iOS
  [2]: https://dribbble.com/shots/1199943-Hexagonal-flat-menu