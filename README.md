# paywitheasebuzz-android-lib
Easebuzz payment api android kit

# Basic steps to integrate PaywithEaseBuzz payment kit for android.

 1.Copy peb-lib.aar file into app/libs/ folder of your application.

 2.Modify build.gradle(module) file in the below section.<br/>
                - defaultConfig { },<br/>
                - repositories{ } ,<br/>
                - Add all required dependencies.<br/>
                                         
 3.Below are the dependancies required for smooth payment process.<br/>
                - compile(name: 'peb-lib', ext: 'aar') <br/>
                - compile 'com.android.support:cardview-v7:28.0.0'<br/>
                - compile 'com.android.support:recyclerview-v7:28.0.0'<br/>
                - compile 'com.squareup.okhttp:okhttp:2.4.0'<br/>
                - compile 'com.android.support:multidex:1.0.1'<br/>
                - compile 'com.squareup.okhttp:okhttp-urlconnection:2.2.0'<br/>
                - compile 'com.squareup.retrofit2:retrofit:2.3.0'<br/>
                - compile 'com.squareup.retrofit2:converter-gson:2.3.0'<br/>
                
                
##### Note : Please use Picasso library version : 2.71828, Old Picasso library version will not give you smooth payment process.


4.Initiate payment request from your application.
                 - On click of pay button of your app you need to start PWECouponsActivity  and require to pass 
                  the necessary parameters to PWECouponsActivity using Intent.
                  (Use startActivityForResult()  method to start the Activity).


5.Handle the response of the payment process.
             - After the transaction has initiated using startActivityForResult() method, your app must override the 
                 OnActivityResult() method of Activity class. This method will receive the status and response of 
                 the transaction.




The step by step detailed procedure to integrate the kit is mentioned in the documentation.pdf file. You can download it from 
  https://github.com/easebuzz/paywitheasebuzz-android-lib/blob/master/documentation.pdf.


