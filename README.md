## SugrMon
Your diabetes monitor


### General information
<b>This application needs a [Nightscout](https://nightscout.github.io/) server to fetch the blood glucose data from !</b>


### Settings screen
![Settings1](https://github.com/HanSolo/Sugr-Mon/raw/main/screenshots/Settings1.png)
![Settings](https://github.com/HanSolo/Sugr-Mon/raw/main/screenshots/Settings2.png)
In the settings screen you need to add the URL of your nightscout server. If you have configured an 
API secret and Token, you can put it in the right fields.
You might select a unit that will be used in SugrMon, either [mg/dl] (default) or [mmol/l].
The sliders in the Glucose Ranges section can be used to adjust your personal preferences. The default 
values are defined as follows:
- Critical Low         55 mg/dl (cannot be changed)
- Acceptable Low   60 -70 mg/dl
- Min good         70- 90 mg/dl
- Max good        120-180 mg/dl
- Acceptable High 120-250 mg/dl
- Critical High   250-350 mg/dl
In the Notifications sections you can define if you would like to receive push notifications with 
alerts for the following situations:
- The current blood glucose value is below the defined Acceptable Low value and 55 mg/dl
- The chance that the next blood glucose value is below 55 mg/dl
- The current blood glucose value is critical which means below 55 mg/dl
For the critical low notification you can also switch on Critical which means this notification will
be send as so called "Critical Alert Notification". These notifications will even be delivered if you are in
"Do not disturb" mode or the phone is set to quite mode. This can be very useful over night, where you definitely
want to receive a notification in case the blood glucose value is critical low. In this case the phone will play a
special tone that is louder than normal and should wake you up when asleep.
For the critical notification you could also define the volume that will be used for the notification, the default value is 0.5.
If you would like to know what the critical alert sound sounds like, you can press the play button and it will play the sound.


### Main screen
![MainScreen](https://github.com/HanSolo/Sugr-Mon/raw/main/screenshots/MainScreen.png)

This screen shows you the most important information at a glance. You can find information about:
- Current blood glucose value incl. trend
- Current unit
- Average blood glucose value for today
- Percentage of time in range (TIR) for today
- The HbA1c (based on the values from the last 30 days)
- Percentage of time in range (TIR) for the last 30 days

The background color of the upper part will change with the current blood glucose value.
The available colors are as follows:
- RED (blood glucose too high or too low)
- ORANGE (blood glucose high or low)
- YELLOW (blood glucose acceptable high or acceptable low)
- GREEN (blood glucose good)

The values for the different ranges can partly be adjusted in the settings.

You will find a line of colored squares for the last 30 days which shows the average value for
each day by it's color. The same colors will be used as for the current value e.g. if the average
value of a day was high, the square will be orange.

In the middle part of the main screen you will see two charts, the bar chart on the upper area
shows the deltas between two measured blood glucose values. This chart can help you to estimate the
next value (esp. if it drops quickly it can help you to be prepared in case the value will be too low soon).

Below the bar chart you will find a line chart that shows the measured blood glucose values as dots with
a fill color defined by the value. You will also find the actual number above each dot.

In the line chart you will also find a green area which indicates the "good range" of blood glucose values.
The x-axis of the charts will show you the time. 

Both charts can be scrolled horizontally and will contain the values of the last 24 hours.

In the bottom of the screen you will find multiple buttons, the first button on the left will lead you to the
selected interval screen where you can see the last 3/6/12 hours as a linechart or poincare plot.
The second button will lead you to the statistics screen where you will further information about daily average
values, CGM statistics etc.
With the third control from the left you can define the number of hours the main screen will show you at once.
And the fourth button with the gear icon will lead you to the settings screen.


### Selected interval screen
![Linechart](https://github.com/HanSolo/Sugr-Mon/raw/main/screenshots/IntervalLinechart.png)
In this screen you can select an interval of either the last 24 hours, 12 hours, 6 hours or 3 hours.
Once selected, the values from that interval will be drawn in a line chart. This can give you an idea
about the values of the selected interval at a glance. Again the x-axis shows the time.
You can toggle the view between a line chart and a poincare plot by tapping on the chart itself.
The poincare plot looks as follows:
![Poincare](https://github.com/HanSolo/Sugr-Mon/raw/main/screenshots/IntervalPoincare.png)

### Statistics screen
![Statistics1](https://github.com/HanSolo/Sugr-Mon/raw/main/screenshots/Statistics1.png)
The statistics screen contains four diagrams, the first one on top shows you the min and max blood
glucose values for the last 30 days as dots that are vertically connected by a thin line.
The average blood glucose values of the last 30 days will be shown as a line chart. On top you can 
see the range of dates that is visualized and the average value for that range.

The second diagram will show you the median (black line) of the last 30 days and also the values in the
P10-P90 range (lighter blue) and in the P25-P75 range (darker blue).

![Statistics2](https://github.com/HanSolo/Sugr-Mon/raw/main/screenshots/Statistics2.png)
The third diagram shows you the percentage of the time you spend in the different ranges. The ranges are:
- Too High
- High
- Acceptable High
- Normal
- Acceptable Low
- Low
- Too Low
As mentioned above, some of these ranges can be adjusted in the settgins. The diagram is based on the
last 30 days. And it will shows in which range you spend the most time during the last 30 days.

### Histories screen
The histories screen will show you the history of the time in range (TIR), the daily average and the HbA1c values
for the last 365 days. The first time you start the app, it will fetch the entries from the last 30 days and will
add the time in range and daily averages for this period to the chart. 
Because the HbA1c value is based on the last 30 days in this app, you will only see one value here at the first
start.
The app will now record one value every day so that you will see the whole history of the three parameters after
365 days of use.
These diagrams can be useful to see the impact of either seasonal behavior (summer/winter) or the effect of holidays
etc.
![History1](https://github.com/HanSolo/Sugr-Mon/raw/main/screenshots/Histories1.png)
![History2](https://github.com/HanSolo/Sugr-Mon/raw/main/screenshots/Histories2.png)

### Widgets
![Widgets](https://github.com/HanSolo/Sugr-Mon/raw/main/screenshots/Widgets.png)
The SugrMon application comes with two different widgets that you can see on the screenshot. Again the
color of the widget gives you an idea about the blood glucose value.
<b> Updating widgets is done by iOS and will be in best case happen every 30 minutes</b>

### Lockscreen widgets
![LockscreenWidgets](https://github.com/HanSolo/Sugr-Mon/raw/main/screenshots/LockscreenWidgets.png)
The application provides two different lockscreen widgets. They both show the blood glucose value and
the trend and the bigger one also shows the time of the value and the HbA1c.
