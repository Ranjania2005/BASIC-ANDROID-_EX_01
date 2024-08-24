# BASIC-ANDROID-_EX_01_Implementation of a Hello world Activity using all lifecycles methods using Android Studio.


## AIM:
To create Hello world Activity using all lifecycles methods to display messages using android studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM
### DEVELOPED BY : RANJANI A
### REGISTER NO: 212223230170

### MainActivity.java:
```
package com.example.myfirstapp;

import android.os.Bundle;
import android.widget.Toast;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
            Toast t=Toast.makeText(getApplicationContext(),"OnCreate Called",Toast.LENGTH_SHORT);
            t.show();
    }
    protected void onStart(){
        super.onStart();
        setContentView(R.layout.activity_main);
        Toast t=Toast.makeText(getApplicationContext(),"OnStart Called",Toast.LENGTH_LONG);
        t.show();
    }
    protected void onResume(){
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast t=Toast.makeText(getApplicationContext(),"OnResume Called",Toast.LENGTH_LONG);
        t.show();
    }
    protected void onRestart() {
        super.onRestart();
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(), "OnRestart Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onPause() {
        super.onPause();
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(), "OnPause Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onStop() {
        super.onStop();
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(), "OnStop Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onDestroy() {
        super.onDestroy();
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(), "OnDestroy Called", Toast.LENGTH_LONG);
        t.show();
    }
}

```
### Activity_Main.XML:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Button"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.5" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.453" />


</androidx.constraintlayout.widget.ConstraintLayout>
```
## OUTPUT:
![exp11](https://github.com/user-attachments/assets/c36aed50-7126-4d02-87ef-799e19f9b24a)

![exp12](https://github.com/user-attachments/assets/4f2e92fe-0958-4b0d-a7d9-341f7ce1ed37)

![exp13](https://github.com/user-attachments/assets/6cfea9bd-bf47-4691-9482-aab6a75f94f6)

![exp14](https://github.com/user-attachments/assets/e6580b57-d31e-4220-936b-c01f9740a030)

## RESULT:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.

