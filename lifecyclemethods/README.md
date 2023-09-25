# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
## Activity_main.xml:
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="40dp"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>

## MainActivity.java:
package com.example.myapplication;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart() {
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    @Override
    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause() {
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume() {
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop() {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onDestroy() {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }
}


Developed by:V.Natchathira Rajan

Registeration Number : 212221040112

## OUTPUT

![image](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/a2482c99-ac97-4470-97a7-70a742b84435)
![image](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/a85ee5ea-0b2b-4055-b0c5-104151bbc0bd)
![image](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/37b6b016-0af4-48da-be8b-be7a93a8525f)

![WhatsApp Image 2023-08-30 at 13 38 32](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/70d48e7a-e006-45f3-8bee-cb1d7590c018)
![WhatsApp Image 2023-08-30 at 13 38 32](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/592b9026-153f-4958-886c-411a44032dc3)
![WhatsApp Image 2023-08-30 at 13 38 32](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/69b02f5c-6ed4-4b6e-af9c-82bf0b1f752c)
![WhatsApp Image 2023-08-30 at 13 38 32](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/79e6335f-774c-43e5-ad0b-d323ff545eb4)
![WhatsApp Image 2023-08-30 at 13 38 32](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/a3514219-a312-4259-a32a-e5dfed6f2c29)
![WhatsApp Image 2023-08-30 at 13 38 32](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/872f57fc-7aa1-446f-b59f-6b098827a398)
![WhatsApp Image 2023-08-30 at 13 38 32](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/1e24b153-c6be-44b9-8f75-6882a41129df)
![WhatsApp Image 2023-09-03 at 14 54 00](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/681c5a9a-af98-49dd-b002-05011013fbb4)




## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
