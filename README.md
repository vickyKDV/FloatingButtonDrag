# FabDagger

![alt text](https://raw.githubusercontent.com/vickyKDV/CircleRectImageView/vickyKDV-imG1/Screen%20Shot%202019-11-03%20at%2021.08.57.png)

   Cara implementasi
   
   
   Set pada build.gradle application
   
     allprojects {
          repositories {
             ...
             ...
             maven { url "https://jitpack.io" }

          }
      }
    
   Set pada build.gradle module
    
    dependencies {
        ...
        ...
        implementation 'com.github.vickykdv:FloatingButtonDrag:1.0'
    }
    
    
  Implementasi pada XML ( Letakan didalam parent view )
  
     <?xml version="1.0" encoding="utf-8"?>
      <RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
          xmlns:app="http://schemas.android.com/apk/res-auto"
          xmlns:tools="http://schemas.android.com/tools"
          android:layout_width="match_parent"
          android:layout_height="match_parent">

          <com.vickykdv.fabdragger.FabButtonDragger
              android:layout_width="wrap_content"
              android:layout_height="wrap_content" 
              android:src="@android:drawable/ic_input_add"
              />

      </RelativeLayout>

