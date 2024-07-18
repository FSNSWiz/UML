```mermaid
    classDiagram

    class Lowrider{
        numTires short
        hydraulics boolean
        roofType string
        loudSpeakers boolean
        hop()
        lights()
        drive()
    }

class Lowridercar{
    numSeats short
    numBatteries short
    rimType string
    threewheel()
    driversideup()
    passengersideup()
}
Lowrider <|-- Lowridercar

class Lowriderbike{
groupSize short
handlebarLength int
bags boolean
helmet boolean
wheelie()
enginerev()
indicateturning()
}
Lowrider <|-- Lowriderbike

class Customizedtrucks{
liftedTruck boolean
loweredTruck boolean
}
Lowrider <|-- Customizedtrucks

class Racecar{
engineType string
speed int
aerodynamic boolean
weight short
accelerate()
crash()
tirechange()
}

class Hotrod{
    tireSize int
    carSpeed short
    flameDecor boolean
    exposedEngine boolean
    race()
    enginerev()
    Nitro()
}
Racecar <|-- Hotrod