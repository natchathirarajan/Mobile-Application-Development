# Ex.No: 2 To develop an application that uses GUI Components with Fonts and Colors. 
Note: Create button for colors and fonts while clicking color or font button should change 


## AIM:

To create an application that uses GUI Components with Fonts and Colors using Android Studio. 

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
Program to print the text “GUIcomponent”.
## Activity_main.xml:
<?xml version="1.0" encoding="utf-8"?>

<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"

xmlns:app="http://schemas.android.com/apk/res-auto"                                                                                     

xmlns:tools="http://schemas.android.com/tools"    

android:layout_width="match_parent"

android:layout_height="match_parent"    

tools:context=".MainActivity">
    

    <Button   
        android:id="@+id/colorButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_centerHorizontal="true"
        android:layout_marginStart="120dp"
        android:text="Change Color"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/fontButton"
        app:layout_constraintVertical_bias="0.082" />

    <Button
        android:id="@+id/fontButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/colorButton"
        android:layout_centerHorizontal="true"
        android:layout_marginStart="120dp"
        android:layout_marginTop="120dp"
        android:text="Change Font"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/fontButton"
        android:layout_centerHorizontal="true"
        android:text="Hello World!"
        android:textSize="40sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.435"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.325" />

</androidx.constraintlayout.widget.ConstraintLayout>

## MainActivity.java:
package com.example.Implicitintent;

import androidx.appcompat.app.AppCompatActivity;

import android.graphics.Color;

import android.graphics.Typeface;

import android.os.Bundle;

import android.view.View;

import android.widget.Button;

import android.widget.TextView;

public class MainActivity extends AppCompatActivity {

    private Button colorButton;
    
    private Button fontButton;
    
    private TextView textView;
    
    @Override
    
    protected void onCreate(Bundle savedInstanceState) {
    
        super.onCreate(savedInstanceState);
        
        setContentView(R.layout.activity_main);
        
        colorButton = findViewById(R.id.colorButton);
        
        fontButton = findViewById(R.id.fontButton);
        
        textView = findViewById(R.id.textView);
        
        colorButton.setOnClickListener(new View.OnClickListener() {
        
            @Override
            
            public void onClick(View v) {
            
                changeTextColor();
                
            } });

        fontButton.setOnClickListener(new View.OnClickListener() {
        
            @Override
            
            public void onClick(View v) {
            
                changeFont();
                
            }
        });
    }
    private void changeTextColor() {
    
        int randomColor = Color.rgb(
        
                (int) (Math.random() * 256),
                
                (int) (Math.random() * 256),
                
                (int) (Math.random() * 256)
        );
        textView.setTextColor(randomColor);
    }
    private void changeFont() {
    
        Typeface[] fontStyles = new Typeface[]{
        
                Typeface.DEFAULT,
                
                Typeface.DEFAULT_BOLD,
                
                Typeface.MONOSPACE,
                
                Typeface.SANS_SERIF,
                
                Typeface.SERIF
                
        };

        int randomIndex = (int) (Math.random() * fontStyles.length);
        Typeface selectedFont = fontStyles[randomIndex];
        textView.setTypeface(selectedFont);}
   }


Developed by: V.Natchathira Rajan
Registeration Number : 212221040112

## OUTPUT

![WhatsApp Image 2023-09-05 at 14 53 11](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/0e2355e4-8190-45a0-9d30-8e691e576580)
![WhatsApp Image 2023-09-05 at 14 53 09](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/1bc4d26b-7676-4ba4-ba38-3de382123b66)
![WhatsApp Image 2023-09-05 at 14 53 09](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/4f5f5ac0-46ea-4fd5-8603-2ea4b87a71d1)
![WhatsApp Image 2023-09-05 at 14 53 10](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/acda0ba9-46b4-43c7-8d02-26975084b174)
![WhatsApp Image 2023-09-05 at 14 53 10](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/2494ec43-f2fe-44b5-8ce8-a6c66d27a296)
![WhatsApp Image 2023-09-05 at 14 53 10](https://github.com/ThiruThanikaiarasu/Mobile-Application-Development/assets/126568917/abed0926-7329-4f4e-a607-b59ffee7a220)



## RESULT
Thus a Simple Android Application that uses GUI Components with Fonts and Colors using Android Studio is developed and executed successfully.
