To change time, and other params, select "WeatherController" actor, and see details panel "Default" section for parameters:

![image](https://user-images.githubusercontent.com/37246339/154375033-6795dac1-8cc4-4425-a536-f96fc32ae714.png)

•"Enabled?" will disable weather controller and you will have to set parameters in "MPC_NukeIslandParameterCollection" parameter collection

•"Time Override" "Override Time?" parameters are mainly for testing, its there so you can set time and update sky in editor (separate from parameter collection value), not only during gameplay

•"Use Low Rez Rain When Low Effects Quality" and "Use Low Rez Rain All the Time" parameters explanation: there is high quality rain niagara system but its too demanding on performance so I just disabled it. You can enable it if you like, but be warned


To change time from from a blueprint, do like this

![image](https://user-images.githubusercontent.com/37246339/154374784-f85166c0-780d-4c94-93c1-0781084480db.png)



To change weather you have to call event "ChangeWeather" in "WeatherController" actor, which is in the level. Like this:

![image](https://user-images.githubusercontent.com/37246339/154374362-15059024-496a-4b65-b2dc-5e07e45bad58.png)
