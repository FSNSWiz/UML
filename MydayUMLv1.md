```Mermaid
    classDiagram

    class Mymorning{
        time short
        date string
        work boolean
        school boolean
        hungry boolean
        checkTime()
        checkDate()
        checkSchedule()
        brushTeeth()
        shave()
    }

    class Workmorning{
        arriveEarly boolean
        arriveOnTime boolean
        arriveLate boolean
        managersOnDuty byte
        drive()
        clockIn()
        speakWithManagers()
        pressureWashOutside()
    }
    Mymorning <|-- Workmorning

    class Schoolmorning{
        breakfastAvailable string
        loginPassword byte
        followingAlong boolean
        watchClassVidLater boolean
        startComputer()
        login()
        openClasstabs()
        startClassCall()
        startAssignments()
    }
    Mymorning <|-- Schoolmorning

    class Myafternoon{
        work boolean
        school boolean
        hungry boolean
        feedPets()
        eat()
        checkTime()
        checkDate()
        checkSchedule()
        parentBaby()
    }

    class Workafternoon{
        RI boolean
        checkPosition string
        checkDrowsy byte
        speakWithManagers()
        clockOutRI()
        clockInPosition()
        helpRestock()
        clean()
        clockOut()
        driveHome()
    }
    Myafternoon <|-- Workafternoon

    class Schoolafternoon{
        pauseAssignment boolean
        checkInClassCall boolean
        checkMissingWork boolean 
        checkGrade byte
        continueAssignment()
        endClassCall()
        startOtherClassCall() 
        endOtherClassCall()
        turnInAssignment()
    }
    Myafternoon <|-- Schoolafternoon

    class Mynight{
        time short
        date string
        happinessLevel byte
        energyLevel byte
        stayingUp boolean
        checkClassDueDates()
        startMovie()
        startSleep()
    }

    class Schoolnight{
        getAhead boolean
        lateWork boolean
        needMoreEnergy boolean
        laptopChargeLvl byte
        chargeLaptop()
        startLateWork()
        drinkEnergyDrink()
        drinkCoffee()
    }
    Mynight <|-- Schoolnight

    class Worknight{
        readyForNextDay boolean
        roomTemp byte
        phoneChargeLvl byte
        startFan()
        chargePhone()
        setAlarms()
        checkWorkSchedule()
    }
    Mynight <|-- Worknight

    class Freenight{
        fanOn boolean
        tvVol byte
        scrollOnPhone boolean
        phoneChargeLvl byte
        gameRemoteChargeLvl byte
        scrollPhone()
        playPhone()
        playConsole()
        chargePhone()
        chargeRemote()
    }
    Mynight <|-- Freenight 