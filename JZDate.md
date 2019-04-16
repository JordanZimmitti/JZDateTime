# JZDate
Class That Handles Date Parsing

#### Setting Up JZDate
JZDate can be set up in two ways, the first way is

    val jzDate = JZDate(1, 1, 2001)
    
The second way is
    
    // Define And Instantiates JZDate Value//
    val jzDate = JZDate() 
    
    // Sets Date Values//
    jzDate.day   = 1
    jzDate.month = 1
    jzDate.year  = 2001
    
The date can be parsed in three different ways: AMERICAN, EUROPEAN, REVERSED
    
    // Gets Date In Format MM/DD/YYYY//
    val date = jzDate.getDate(JZDateFormat.AMERICAN) 
    
    // Gets Date In Format DD/MM/YYYY//
    val date = jzDate.getDate(JZDateFormat.EUROPEAN) 
    
    // Gets Date In Format YYYY/MM/DD//
    val date = jzDate.getDate(JZDateFormat.REVERSED) 
    
#### Getting The Day, Month, Or Year From A Full Date
The first parameter is the full date string<br/> 
The second parameter is the format of the inputted date string<br/>

    // Gets The Day, Month, And Year From The Full Date//
    val day   = JZDate.fullDateToDay("05/05/2005", JZDateFormat.AMERICAN)
    val month = JZDate.fullDateToMonth("05/05/2005", JZDateFormat.AMERICAN)
    val year  = JZDate.fullDateToYear("05/05/2005", JZDateFormat.AMERICAN)
    
#### Getting The Current Date
The parameter is what format the current date should be in<br/>

    // Gets The Current Date In The Different Formats//
    val americanDate = JZDate.getCurrentDate(JZDateFormat.AMERICAN)
    val europeanDate = JZDate.getCurrentDate(JZDateFormat.EUROPEAN)
    val reversedDate = JZDate.getCurrentDate(JZDateFormat.REVERSED)
    
#### Getting The Current Day, Month, Year

    // Gets The Current Day, Month, And Year//
    val currentDay   = JZDate.getCurrentDay()
    val currentMonth = JZDate.getCurrentMonth()
    val currentYear  = JZDate.getCurrentYear()
    
#### Switching A Date Format
The first parameter is the date string<br/>
The second parameter is the format the inputted date is currently in<br/>
The third parameter is the format the inputted date should be switched to<br/>

    // Switches The Date Format From 10/10/2010 to 2010/10/10//
    val switchedDate = JZDate.switchDateFormat("10/10/2010", JZDateFormat.AMERICAN, JZDateFormat.REVERSED)
