# DarioWeekViewDatePicker
An Android week view component for selecting a date

<img src="art/screen0.png" width="200"/>

## Install
root `build.gradle` file:
```gradle
allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}
```

app `build.gradle` file:
```gradle
implementation 'com.github.myDario:DarioWeekViewDatePicker:1.0.3'
```

## Usage
```xml
<com.labstyle.darioweekviewdatepicker.DarioWeekViewDatePicker
    android:id="@+id/datePicker"
    android:layout_width="match_parent"
    android:layout_height="wrap_content" />
```

## Selection change listener
```kotlin
findViewById<DarioWeekViewDatePicker>(R.id.datePicker).onSelectionChanged = { date ->
    // ...
}
```

## Select a date at runtime
```kotlin
findViewById<DarioWeekViewDatePicker>(R.id.datePicker).setSelection(date)
```

## V 1.0.2 Release notes
* Removing scrollview and centering days
* Adding today button
* Adding Today string to date (in case today selected)
* Rename left/right arrows to resolve conflict in code

## V 1.0.3 Release notes
* Revert back scrollview (days kept centered)
* Enlarging today button

## V 1.0.4 Release notes
* add setter for today text resource.
* set date format to be DateFormat.MEDIUM  instead of DateFormat.LONG

## V 1.0.5 Release notes
* add ',' char after "today" to date text

## V 1.0.6 Release notes
* change font weight to date title text
* change date title text margin