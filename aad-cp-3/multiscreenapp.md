# Multiscreen App
  Apps, which are fun and easy to use, can give children's a variety of learning and approaches to keep them engaged and help in enhancing knowledge.
  so thought to make an app  "All in one place, knowledge pool for children".

<img src="https://user-images.githubusercontent.com/69693530/101532230-40469580-39ba-11eb-8c0e-552675bb5b94.gif" width="400" height="550">

## Things you will learn :

  * #### How to manage gradle file.
  * #### Working with Fragments.
  * #### Adding sound to an App.
  * #### Using list, array, loops.
  * #### How to add images and audio.

## Lets deep dive into the topics :

* ### Managing gradle file :
  Gradle file build configurations that are applied to all modules of our app.By adding dependencies ,it becomes easy to include external library in our project.
  To add a dependency, we specify a dependency configuration such as ```implementation``` in the dependencies block of your ```build.gradle``` file.
  here is snippet of ```Build.gradle```(Module:app)
  
```
dependencies {
    implementation fileTree(dir: "libs", include: ["*.jar"])
    implementation 'androidx.appcompat:appcompat:1.2.0'
    implementation 'androidx.constraintlayout:constraintlayout:2.0.4'
    implementation "androidx.cardview:cardview:1.0.0"
    implementation 'com.google.android.material:material:1.2.1'
    implementation 'androidx.legacy:legacy-support-v4:1.0.0'
    implementation 'androidx.gridlayout:gridlayout:1.0.0'
    implementation "androidx.fragment:fragment:$fragment_version"
    implementation 'androidx.navigation:navigation-ui-ktx:2.1.0'
    implementation 'androidx.recyclerview:recyclerview:1.1.0'
    testImplementation 'junit:junit:4.12'
    androidTestImplementation 'androidx.test.ext:junit:1.1.2'
    androidTestImplementation 'androidx.test.espresso:espresso-core:3.3.0'
}
```

* ### Working with Fragments :
### Fragments -
Fragments represents a portion of our app which is reusable.It has its own layout,and lifecycle.They are hosted by an Activity or fragmet.In fragments we need viewpager.

 * To create fragments first we need to add dependency in our ```Build.gradle``` file.
 * The Java controller for a fragmente  ```TabA1``` and its XML layout file ```Fragments_tab_a1```.<br>
 * PageAdapter, this is adapter class. This adapter file will define no. of page exist and  which fragment to display for each page of the adapter by creating this file.
 * To apply this Adapter file, we need to associate the ViewPager with a new instance of our adapter.<br>

### ViewPager -
  * With the help of viewpager we can access the selected page within the ViewPager at any time with the getCurrentItem method which returns the current page.
  * ViewPager also  display a tabbed indicator in order to create tabs to display our fragments.
  ```
    <androidx.viewpager.widget.ViewPager
        android:id="@+id/viewPage1"
        android:layout_width="match_parent"
        android:layout_height="match_parent"/>
       
  ```

* ### Working with Sounds and Images :
 For adding audio we made folder called ```raw``` in res directory and added all th audio to it.And for images we added all the images in floder ```Drawable```.
 
 
###  Contribution in Android App Development under DevIncept 30-DAYS CONTRIBUTOR PROGRAM
#### Nice working with the team and thanks to the organization ``` DevIncept``` for organizing 30-Days contributor Program.
 
 ## Team Members :
 * #### Vineet Joshi (Team Leader)
 * #### Anukrati Rawal
 * #### Amit Kumar Mishra
 * #### Bernotsha 
 
#### ```# OpenSourceContribution```    ```# DevIncept```    ```# 30-Days Contributor Program```


