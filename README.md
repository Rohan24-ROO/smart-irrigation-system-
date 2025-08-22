# smart-irrigation-system using API
  
4 Modes

1.Auto scheduler
2.Weather based water irrigation
3.Manual mode
4.Remote execution

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

every hour the irrigtion system sends sms or whats app message to farmers secondary device about watering updates.


1. Why auto scheduler ?
Ans: The autoscheduler helps when the farmer is outside of the network coverage area or when the farmer is not able to plant the water may be cause of any reason so at that time
so at that time the irrigation project check the spscific requiremnets and then automates the watering system, so like this the farm will be properly maintained and in balance.
sends whats app message once the execution starts.

2. Why weather based water irrigation ?
Ans: In autoscheduler system if the time is not specified the scheduler wont be turned on so, The weather based system plays main role in maintaining the water in the farm
so weather system first check the moisture level of the garden and then based on moisture level and weather condtions it release the water. even if the farmer is not avaialbe to check in th farm
it works automatically. sends whats app message once the execution starts.

3. Why manual mode ?
Ans: Manual mode is helpful when farmer is available for irrgating the farm he can turn on the watering system if he want based on his needs. sends 
whats app message once the execution starts.

4. Why remote execution mode ?
Ans: In remote exceution mode the farmer can control the farm by any device from anywhere in th world with help of the remote connecton. Like when farmer is in kerala and his farm
is in karnataka ad he want to turn on the irrgation system then he have to send then turn on trigger to his mobile which is in karnataka which controls the farm. this methods cheks
if the moisture, temparature and weather are needed as requirement if its true it turns on motor or else it wont.
so when he want to turn it off he can simply send off trigger to his device. sends whats app message once the execution starts.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

1. AutoScheduler: Schedulesr which send whats app message when its time for plant watering and also when plant watering system shutdown time. but first it checks if the time is 
11 Am or 6 Pm and the moisture level and along with that it cheks current weather level. 

Example: Time is 11 Am and moisture is below <30% and weather is sunny. Then the water pump will on and the water will start flowing until the moisture becomes >90% once the mosture reaches the max limit
the pump will turn off and send whats app message with current info like (temp,mositure,motor on/off,next schedule)

Example: Time is 11 Am and the moisture is >80% and weather is cloudy. Then the wate pump will remain off and the water will not be flowing. and if Time is 11 Am and the moisture is <30% and weather is cloudy the schedule will be skipped.

2. Weather based irrigtion system: In this the irrigation system will be turned on if the weather is sunny and the moisture is below than <30% and if the moisture is above than >90%
then irrigation wont be happen based on this moisture and weather the irrigation system will stop.

Example: If the weather is cloudy and the moisture is <30% the irrigation wont be turned on. instead if the weather is sunny and the the mositure is >90% then also it wont execute.
but if the weather is sunny and the moisture level is <30% then ths exceution happens and sms will be sent as well, and if the weather is sunny and the moisture is >90% then the exceution
wont be happen here.

3. Manual mode:
the manual mode will be turned on if the farmer want to turn on the motor and first it cheks if the moisture level are below <30% and weather is sunny, if the same trigger keeps repateing then
the mode will be activated as per rule. if the weather is cloudy or rainy then the trigger will not turned on until the tgrigger is repeated.

Example: if the moisture is <30% and weather is sunny then the manual mode will be turned on and if the weather is sunny and the mpisture is >90% then it wont. but if the tigger is repeted in soecific time
then the waterig system will start.

Example: if the moisture level is <30% and the weather is rainy then the trigger will not start but if the trigger is repeted in specifiv time it will start.

4. Remote execution: In this mode the trigger will be sent to device and if the weather is sunny and moisture is under >30% this will execute or else if the misture is more than >90% then it wont start until the trigger is repeted 
until specific time. 

Example: if the weather is sunny and the moisture is <30% the water system will start on trigger , if the weather is rainy and the and moisture is <30% then the trigger will not be turned on

Example: if the wetaher is sunny and moisture is more than >90% then the trigger will start or else it wont until thr triggers is repeted till specific time.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The LCD screen will show 

system loading.....

moisture level: 30%
Motor On/Off

Next it will show (after 20 seconds)

temparature : 60%
weather: Sunny

schedule: 11 Pm
schedule: 6 Pm


all this info also shows on app as well and tet fomat in whats app message;

moisture level: 30%
Motor: On/Off
temparature : 60%
weather: Sunny
schedule: 11 Pm
schedule: 6 Pm
