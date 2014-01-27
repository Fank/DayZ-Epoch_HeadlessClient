# DayZ-Epoch_HeadlessClient

Headless client support for DayZ Epoch

## Installation (Mission)

Edit the **init.sqf** and add following above `progressLoadingScreen 1.0;`:
```
call compile preprocessFileLineNumbers "headlessclient\compile\init.sqf";
```

So it looks like this:
```
progressLoadingScreen 0.9;
call compile preprocessFileLineNumbers "headlessclient\compile\init.sqf";
progressLoadingScreen 1.0;
```

And add this to the end of the document:
```
[] execVM "headlessclient\init.sqf";
```