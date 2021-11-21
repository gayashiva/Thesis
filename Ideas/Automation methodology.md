202111211158

**Status:** 

**Tags:** 

# [[Automation methodology]]

Since the ice radius and the spray radius depend on each other it is quite complicated to determine the actual freezing rate. The discharge rate determines the spray radius which determines the ice radius. I make the simple assumption that the ice radius is equal to the median of the total spray radius variation. 

Freezing rate depends on the ice radius whereas discharge rate depends on the spray radius.

To have enough area to freeze, we want to increase the ice radius but to reduce water loss, we want to decrease the spray radius. So to achieve a balance between increasing freezing rate and reducing water loss, I have come up with this new strategy:

1. Choose the desired ice radius (median spray radius). For guttannen, this is 8m. This desired ice radius corresponds to the desired freezing rate. So 8m ice radius corresponds to 9 l min-1 freezing rate for Guttannen. So median spay radius is 8m.
2. Assuming fountain runtime is half of the freezing duration (Jan and Feb). The spray radius is greater than the ice radius for a quarter of the freezing duration. We can ensure this using the 25th percentile values of temperature, humidity and mean wind speed (since variation is high here). Lets call these values temp_25, rh_25 and wind_mean respectively. These values correspond to the critical weather conditions beyond which the spray radius is greater than the desired ice radius.
3. Using the simplified energy balance, we find the critical freezing rate per m2 for our critical weather conditions. From the desire discharge rate and the critical freezing rate we obtain the virtual radius reuired. For Guttannen, this is 17 m.
4. We scale the simplified energy balance using this virtual area to obtain the recommended discharge variation required to support our desired ice radius.  



---
# References