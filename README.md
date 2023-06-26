Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.

AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

EQUIPMENTS REQUIRED:

Latest Version Android Studio

ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

PROGRAM:

activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"

    xmlns:app="http://schemas.android.com/apk/res-auto"
    
    xmlns:tools="http://schemas.android.com/tools"
    
    android:layout_width="match_parent"
    
    android:layout_height="match_parent"
    
    tools:context=".MainActivity">
    
    <TextView
        android:layout_width="wrap_content"
        
        android:layout_height="wrap_content"
        
        android:text="Hello World!"
        
        app:layout_constraintBottom_toBottomOf="parent"
        
        app:layout_constraintEnd_toEndOf="parent"
        
        app:layout_constraintStart_toStartOf="parent"
        
        app:layout_constraintTop_toTopOf="parent" />
        
        </android.support.constraint.ConstraintLayout>

  MainActivity.java

  /*
  
Program to print the text “Hello World”.

Developed by: Arun Karthik.V

Registration Number: 212221040018

*/

package com.example.exp1;

import android.os.Bundle;

import android.support.v7.app.AppCompatActivity;

import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    
    protected void onCreate(Bundle savedInstanceState) {
    
        super.onCreate(savedInstanceState);
        
        setContentView(R.layout.activity_main);
        
        Toast.makeText(this, "onCreate Called", Toast.LENGTH_SHORT).show();
        
    }
    
    @Override
    
    protected void onRestart(){
    
        Toast.makeText(this, "onRestart Called", Toast.LENGTH_SHORT).show();
        
        super.onRestart();
        
    }
    
    @Override
    
    protected void onStart(){
    
        Toast.makeText(this, "onStart Called", Toast.LENGTH_SHORT).show();
        
        super.onStart();
    }
    
    @Override
    
    protected void onResume(){
    
        Toast.makeText(this, "onResume Called", Toast.LENGTH_SHORT).show();
        
                super.onResume();
    }
    
    @Override
    
    protected void onPause(){
    
        Toast.makeText(this, "onPause Called", Toast.LENGTH_SHORT).show();
        
        super.onPause();
        
    }
    
    @Override
    
    protected void onStop(){
    
        Toast.makeText(this, "onStop Called", Toast.LENGTH_SHORT).show();
        
        super.onStop();
        
    }
    
    @Override
    
    protected void onDestroy(){
    
        Toast.makeText(this, "onDestroy Called", Toast.LENGTH_SHORT).show();
        
        super.onDestroy();
        
    }
    
}

OUTPUT:

![image](https://github.com/Karthik2821/Hello-world/assets/134921933/f7e8a917-882a-42d3-a981-f694687c132e)

![image](https://github.com/Karthik2821/Hello-world/assets/134921933/48370cc8-34b0-45d2-b574-c79722def412)

![image](https://github.com/Karthik2821/Hello-world/assets/134921933/5ba694cd-4ece-4cf0-a22f-06ca44ab5b0e)  

RESULT:

Thus, a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.















