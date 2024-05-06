
# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:



## PROGRAM:
```
/*
Program to print the text “optionmenu”.
Developed by:Kayyuru Tharani
Registeration Number :212221040080
*/
```

####  activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <androidx.appcompat.widget.Toolbar
        android:id="@+id/toolbar"
        android:layout_width="match_parent"
        android:layout_height="?attr/actionBarSize"
        android:background="?attr/colorPrimary"
        app:title="Options Menu Example"
        app:titleTextColor="@android:color/white" />

</RelativeLayout>
```
#### mainactivity.java:
```
package com.example.menuapp;

import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.Menu;
import android.view.MenuInflater;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);


        androidx.appcompat.widget.Toolbar toolbar = findViewById(R.id.toolbar);
        setSupportActionBar(toolbar);
    }

    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        MenuInflater inflater = getMenuInflater();
        inflater.inflate(R.menu.option, menu);
        return true;
    }
}
```
#### option_xml:
```
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item
        android:id="@+id/action_item1"
        android:title="Item 1" />
    <item
        android:id="@+id/action_item2"
        android:title="Item 2" />
    <item
        android:id="@+id/action_item3"
        android:title="Item 3" />
</menu>
```

## OUTPUT

![Screenshot (418)](https://github.com/KayyuruTharani/menuinandroid/assets/142209319/e16ce87a-c2d9-4ae2-9a1a-dc041d188b81)


![Screenshot (419)](https://github.com/KayyuruTharani/menuinandroid/assets/142209319/322c6a55-9f30-42d3-9686-b51f6d8b5363)

## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.
