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
The parameter is the format for the returned time<br/>

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
    
#### Getting The Hour From The Full Time
The first parameter is the full time string<br/>
The second parameter is the format for the returned hour<br/>

    // Gets The Hour From The Full Time//
    JZTime.fullTimeToHour("13:05", JZTimeFormat.STANDARD)
    
#### Getting The Minute From The Full Time
The parameter is the full time string<br/>

    // Gets The Minute From The Full Time
    JZTime.fullTimeToMinute("13:05")
    
#### Getting The Current Hour
The parameter is the format for the returned hour<br/>

    // Gets The Current Hour//
    JZTime.getCurrentHour(JZTimeFormat.STANDARD)
    
#### Getting The Current Minute
    
    // Gets The Current Minute//
    JZTime.getCurrentMinute()
    
#### Getting The Current Time
The parameter is the format for the returned time<br/>

    // Gets The Current Time//
    JZTime.getCurrentTime(JZTimeFormat.MILITARY)
