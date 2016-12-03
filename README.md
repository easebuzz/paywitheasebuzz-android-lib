# paywitheasebuzz-android-lib
Easebuzz payment api android kit

# Basic steps to integrate PaywithEaseBuzz payment kit for android.

 1.Copy peb-lib.aar file into app/libs/ folder of your application.


 2.Modify build.gradle(module) file in the below section.
               - defaultConfig {  },
                - repositories{ } , 
                - Add all required dependencies.


3.Initiate payment request from your application.
                 - On click of pay button of your app you need to start PWECouponsActivity  and require to pass 
                  the necessary parameters to PWECouponsActivity using Intent.
                  (Use startActivityForResult()  method to start the Activity).


4.Handle the response of the payment process.
             - After the transaction has initiated using startActivityForResult() method, your app must override the 
                 OnActivityResult() method of Activity class. This method will receive the status and response of 
                 the transaction.




The step by step detailed procedure to integrate the kit is mentioned in the documentation.pdf file. You can download it from 
  https://github.com/easebuzz/paywitheasebuzz-android-lib/blob/master/documentation.pdf.


