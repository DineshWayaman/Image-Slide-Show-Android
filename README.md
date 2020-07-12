# Image-Slide-Show-Android
Android application image slide slow follow my commands one by one

This is an amazing image slider for the Android .

You can easily load images with your custom layout, and there are many kinds of amazing animations you can choose.
   
         implementation 'com.github.denzcoskun:ImageSlideshow:0.0.6'
         
New Feautures
      Ability to disable default indicator.
      
First put the slider view in your layout xml :   
            
            <com.denzcoskun.imageslider.ImageSlider
              android:layout_width="350dp"
              android:layout_height="200dp"
              app:placeholder="@drawable/download"
              app:error_image="@drawable/download"
              android:gravity="center"
              android:id="@+id/slider"
              app:auto_cycle="true"
              app:delay="0"
              app:period="1000"
              app:corner_radius="10"/>
              
  
Next step
  Add folloeing code to your Java file inside: 
       
        ImageSlider imageSlider;
         
        imageSlider = (ImageSlider)findViewById(R.id.slider);
        
        List<SlideModel> slideModels = new ArrayList<>();
        slideModels.add(new SlideModel("//your image link here","Rice Recipes"));
        slideModels.add(new SlideModel("//your image link here","Meat Recipes"));
        slideModels.add(new SlideModel("//your image link here","Cake Recipes"));
        slideModels.add(new SlideModel("//your image link here","Fruit Recipes"));
        slideModels.add(new SlideModel("//your image link here","Vegetarian Recipes"));
        imageSlider.setImageList(slideModels,true);
        
        
 Contribute
  Suggestions and pull requests are always welcome
          
