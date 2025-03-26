
# Ex.No:1 a.) Implementation of a Hello world Activity using all lifecycles methods using Android Studio.

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

## PROGRAM:
 ```
/*
Program to implement a Hello world Activity using all lifecycles methods using Android Studio .
Developed by: NIVESHA P
RegisterNumber:  212222040108
*/
```

## activitymain.xml:

```
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
android:id="@+id/main"
android:layout_width="match_parent"
android:layout_height="match_parent"
android:orientation="vertical"
android:padding="16dp">
<!-- A simple TextView to display a message -->
<TextView
android:id="@+id/main_text"
android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:text="Hello, World!"
android:textSize="24sp"
android:layout_gravity="center_horizontal"
android:paddingBottom="16dp"/>
<!-- A Button that the user can press -->
<Button
android:id="@+id/main_button"
android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:text="Click"
android:onClick="one1"
android:layout_gravity="center_horizontal"/>
</LinearLayout>

```
## MainActivity.java:
```
package com.nextstep.application;
import android.annotation.SuppressLint;
import android.content.DialogInterface;
import android.os.Bundle;
import android.widget.ImageView;
import android.widget.Toast;
import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AlertDialog;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;
public class MainActivity extends AppCompatActivity {
@SuppressLint("MissingInflatedId")
@Override
protected void onCreate(Bundle savedInstanceState) {
super.onCreate(savedInstanceState);
setContentView(R.layout.activity_main);
Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG).show();}
@Override
protected void onStart() {
super.onStart();
Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG).show();
}
@Override
protected void onResume() {
super.onResume();
Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG).show();
}
@Override
protected void onPause() {
super.onPause();
Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG).show();
}
@Override
protected void onStop() {
super.onStop();
Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG).show();
}
@Override
protected void onRestart() {
super.onRestart();
Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG).show();
 }
@Override
protected void onDestroy() {
super.onDestroy();
Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG).show();
}}
```
## activitymain.xml:
```
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
android:id="@+id/main"
android:layout_width="match_parent"
android:layout_height="match_parent"
android:orientation="vertical"
android:padding="16dp">
<!-- A simple TextView to display a message -->
<TextView
android:id="@+id/main_text"
android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:text="Hello, World!"
android:textSize="24sp"
android:layout_gravity="center_horizontal"
android:paddingBottom="16dp"/>
<!-- A Button that the user can press -->
<Button
android:id="@+id/main_button"
android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:text="Click"
android:onClick="one1"
android:layout_gravity="center_horizontal"/>
</LinearLayout>

```
## OUTPUT:

![Screenshot 2024-08-28 215626](https://github.com/user-attachments/assets/531b2bea-362d-48f1-b164-ff1f81191329)

![Screenshot 2024-08-28 215647](https://github.com/user-attachments/assets/282178c3-34fc-4407-9afc-a5c39ae127b0)

![Screenshot 2024-08-28 215712](https://github.com/user-attachments/assets/8cbeb223-2568-45a6-876d-9cdcb3b435bf)

## RESULT:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.
