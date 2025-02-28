# flight-simulator-cessna172
This C++ program simulates the flight of a Cessna 172, incorporating randomized weather conditions, fuel consumption, and real-time adjustments based on environmental factors. Below is a breakdown of the key components:

🌤️ Weather System
The Weather class generates random weather conditions affecting the flight:

Wind Speed & Direction: Affects plane heading and power adjustments.
Precipitation: Can be Clear, Rain, or Snow.
Turbulence Probability: 30% chance of severe turbulence, moderate if wind > 30 km/h.
📌 Effect on Flight:

High winds force adjustments in power and heading.
Severe turbulence makes the plane drop altitude.
ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ

🛩️ Cessna 172 Class (Flight Mechanics)
The Cessna172 class models the aircraft's behavior, handling takeoff, flight adjustments, and landing.

✈️ Key Properties:
speed: The current speed of the aircraft.
altitude: The aircraft’s altitude above ground.
power: Engine power level in percentage.
fuel: Remaining fuel in liters.
remainingDistance: Distance left to reach the destination.
inFlight: Determines whether the flight is ongoing.
📌 Takeoff Sequence:

The aircraft gradually increases power and speed.
Once it reaches 120 km/h, the plane takes off and ascends to 3,000 meters cruise altitude.
📌 In-Flight Adjustments:

The plane adjusts heading and power depending on the wind direction & speed.
Turbulence can cause altitude changes.
Fuel consumption is tracked per iteration.
If fuel runs out, the plane issues an emergency landing warning.
📌 Landing Procedure:

The plane gradually reduces speed and altitude.
Once it reaches 130 km/h, the landing is completed
ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ

🎲 Randomized Flight Dynamics
The flight distance is randomly assigned between 100-1000 km.
Weather changes periodically during the flight, requiring the plane to adjust dynamically.
ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ

🔥 Summary
        ✅ Realistic flight physics (lift, drag, speed thresholds)
        ✅ Random weather conditions impacting flight performance
        ✅ Real-time fuel consumption tracking
        ✅ Dynamic autopilot adjustments for turbulence & wind
        ✅ Landing sequence & emergency handling
