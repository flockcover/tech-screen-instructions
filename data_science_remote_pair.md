# Data Science Screen Instructions

Bob's Epic Drone Shack Inc. manufacturers drones and offers realtime weather reports for drones. They have made an API available at [bobs-epic-drone-shack-inc.herokuapp.com](https://bobs-epic-drone-shack-inc.herokuapp.com/) which provides a weather report for the current hour and drone specifications.

GET -> /api/v0/weather

GET -> /api/v1/drone/:id

We have pulled down an example of the response from each API in JSON format.
```
    # Weather
    {
    	"windSpeed": 8, # (m/s)
    	"temperature": 2, # (degreesC)
        "rainfallProbability": 0.2, # (%)
    	"visibility": 500 # (m)
    }
```
```
    # Drone
    {
    	"mass": 3, # (kg)
    	"price": 2000, # (£)
        "maxWindResistance": 10, # (m/s)
    	"minimumOperatingTemperature": -10, # (degreesC)
    	"maximumOperatingTemperature": 40 # (degreesC)
    }
```

Flock has decided to use the data from Bob's Epic Drone Shack to make a new risk algorithm for drones. The algorithm will calculate the monetary loss that Flock expects a drone flying for 1 hour to incur, the expected loss.

Your task is to produce an algorithm which takes a drone and the current time as an input, producing the probability of the drone crashing and the expected loss in £ as an output. You should only account for the expected damage to the drone when quantifying the expected loss.

You should also calculate the probability of the drone crashing and the expected loss in £ for the example input data given.

### Input

- Weather
    - windSpeed (m/s)
    - temperature (degreesC)
    - rainfallProbability (%)
    - visibility (m)

- Drone Specs
    - mass (kg)
    - price (£)
    - maxWindResistance (m/s)
    - minimumOperatingTemperature (degreesC)
    - maximumOperatingTemperature (degreesC)

### Output

- Probability of drone crash (%)
- Expected loss (£)

You do not have any data available to train the algorithm on, but should account for this becoming available in the future.

This can be solved using any tool or environment you choose, e.g. Jupyter notebooks, R studio, PyCharm ...

You have access to google and any other tool you would normally have access to under typical work conditions.
