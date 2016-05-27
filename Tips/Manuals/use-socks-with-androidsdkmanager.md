VM has environment variable for proxy.

Default port for socks proxy is 1080, If you are running your proxy in another port you have to tell jvm which port is it.

[Linux]

 export _JAVA_OPTIONS="-DsocksProxyHost=<YourProxyHost> -DsocksProxyPort=<YourProxyPort>"
 
 [Windows]
 
 set _JAVA_OPTIONS="-DsocksProxyHost=<YourProxyHost> -DsocksProxyPort=<YourProxyPort>"
 
 And run android sdk manager in current session.
 
 [Linux]
 
  bash /path/to/sdk/tools/android
  
  [Windows]
  
   c:\path\to\android.exe
