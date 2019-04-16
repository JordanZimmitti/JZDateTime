# JZTime
Class That Handles Time / Time Difference

#### Setting Up JZTime
JZTime can be set up in two ways, the first way is

    // Define And Instantiates JZTime Value// 
    val jzTime = JZTime(13, 5, 10, 5)
    
The second way is

    //Define And Instantiates JZTime Value// 
    val jzTime = JZTime() 

    // Sets End-Time Values//
    jzTime.endTimeHour   = 13
    jzTime.endTimeMinute = 5

    // Sets Start-Time Values//
    jzTime.startTimeHour   = 10
    jzTime.startTimeMinute = 5
    
#### Parsing The End-Time And Start-Time
The parameter is what format the time should be in<br/>

    // Gets The Start-Time In Format HH:mm//
    jzTime.getStartTime(JZTimeFormat.MILITARY)
    
    // Gets The End-Time In Format HH:mm aa//
    jzTime.getEndTime(JZTimeFormat.STANDARD)
    
#### Getting The Time Difference Between Start-Time And End-Time In Hours And Minutes

    // Gets The Time Difference//
    jzTime.getTimeDifference()
    
#### Getting The Time Difference Between Start-Time And End-Time In Minutes

    // Gets The Time Difference In Minutes//
    jzTime.getTimeDifferenceInMin()
