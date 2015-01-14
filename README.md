Adaptation of the Nymi BasicExample app as distributed in NymiSDK-Android-2.0-Build38.

Changed to interface to a Nymi band:

	Out of Box configuration, as downloaded, uses the Nymulator native libraries lib_nymi_sdk_net.so
	Update native libraries to  use those that interface with real Nymi bands.  
		Use: lib_nymi_sdk.so  Removed lib_nymi_sdk_net.so net libraries 
	Updated jar: Removed NCL.net.jar, Added NCL.native.jar
	Invalidated caches in Android Studio, restarted Studio
	Updated app/build.gradle - 
		Replaced entry "compile files('libs/NCL.net.jar')" with "compile files('libs/NCL.native.jar')"

Using app to provision a band has intermittent success.  
Using a Samsung Galaxy Tab4, SM-T230NU, 4.4.2, Build KOT49H the app ALWAYS disconnects during the 'Agree' step.
Using a Samsung Galaxy S3, 4.4.2 the app is successful about half the time.

 
