# Helium Hotspots Simulator

A script that reads the data from your Google map and
helps you find the perfect spot for your next hotspot(s) by
showing the distances to the other hotspots in an *X* meters
range, highlighting the ones that are closer than 300 meters
and showing the number of hotspots / layer in the *X* meters
range.

### e.g. [The map of Bucharest](https://www.google.com/maps/d/u/0/viewer?mid=1XRWBaTQ8lfD94CyVjmM71D6k5s808Hs5&ll=44.428648689281395%2C26.095210930261587&z=13&fbclid=IwAR3qk2Xtk1kGEZYZLhdqVFPEKeTZlI5nHJeQK2SZ6CS0fjLfFyAkBBk6L_4)

![Bucharest](https://github.com/botondszekeres/helium_map/blob/main/hotspot_details.PNG)

## Setup
- Open the following link: https://mybinder.org/v2/gh/botondszekeres/helium_map/c898a4d5905ade608aa1b6c2e6d3f91a1eb5b907?filepath=helium_map.ipynb
- Replace the URL with your map's URL
  ```
    ################# EDIT THIS #################
    url = 'https://www.google.com/maps/d/u/0/viewer?mid=1XRWBaTQ8lfD94CyVjmM71D6k5s808Hs5&ll=44.428648689281395%2C26.095210930261587&z=13&fbclid=IwAR3qk2Xtk1kGEZYZLhdqVFPEKeTZlI5nHJeQK2SZ6CS0fjLfFyAkBBk6L_4'
    #############################################
  ```
- Set the range and replace the coordinates and names
  of the hotspots with the ones you want to simulate.
  Format: list of `([lat, lng], 'name')` separated by commas.
  ```
    ################# EDIT THESE #################
    range = 800
    simulated_hotspots = [
        ([44.416885, 26.0292903], 'SIM_1'),
        ([44.41903352271246, 26.023432370792236], 'SIM_2')
    ]
    ##############################################
  ```
- Hit the `>>` button, then the `Restart and Run All Cells` and wait a few seconds
