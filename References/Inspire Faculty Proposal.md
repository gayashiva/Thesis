
202207191435
**Tags:** 

# [[Inspire Faculty Proposal]]

## Origin of the proposal
Irrigated agriculture is crucial for the livelihood security of mountain communities.
Using meltwater from glaciers, snow and permafrost, mountain dwellers have
developed sophisticated techniques to cope with recurrent water scarcity caused
by glacial retreat, glacier thining, and seasonal snow-cover dynamics. Artificial ice
reservoirs (AIRs) are a key example of such a water storage technology. More than 500 mountain farmers in Ladakh build these ice structures. These seasonal ice
reservoirs increase meltwater availability during the critical period of water scarcity
in spring. To assess the role of AIRs within the water resource management
of mountain villages under a changing climate, they need to be represented in
integrated modelling frameworks like glacier models. To reduce their water losses,
their construction strategies need to be made sensitive to the location’s weather
conditions and water availability. 


## Objectives


## Brief outline of the methodology

The methodology followed will be similar to the one used in our previous research. We will develop software and hardware tools that quantify volume evolution of ice terraces and improve their water-use efficiency.

In a first step, a measurement campaign will be conducted on existing ice terrace construction locations using weather stations, discharge loggers and drones to acquire calibration and validation datasets for the ice terrace software developed. In a second step, a construction campaign will be conducted using an automation hardware designed to implement water supply management using the ice terrace software. In a third step, an AIR suitability metric will be developed that integrates with existing water scarcity metrics to identify regions beyond Ladakh that will benefit from this water storage technology.

## Significance of the proposal in the context of current status in the field


## Prospects of this work for extending it as a long term project

By definition, all glaciers, including the smallest ones, are bodies of sedimentary
ice which were built up by progressive snow compaction and firnification and flow
downhill under the influence of gravity [4]. Hence, because of their genesis and
composition, AIRs differ from glaciers. But when classified in terms of size and
survival duration, AIRs exhibit similar characterestics to very small glaciers. The
glossary of glacier mass balance and related terms by Cogley et al. [11] defines very
small glaciers or glacierets as follows:

A very small glacier, typically less than 0.25 km2 in extent, with no
marked flow pattern visible at the surface. To qualify as a glacieret, an
ice body must persist for at least two consecutive years. Glacierets can
be of any shape, and usually occupy sheltered parts of the landscape.
Windborne snow and avalanches can be dominant contributors to the
accumulation of glacierets.

This rather broad definition of glacierets or very small glaciers may be the one best
suited for AIRs. Ice terraces have been measured to have areas upto 0.15 km2 by
Nüsser et al. [30]. Ice stupas have been observed to last for two consecutive years.
However, most AIRs are neither so large or last so long.

Based on this definition, we can define "artificial glaciers" as ice bodies that are both
larger in area and last longer than two consecutive years. Manmade ice structures
can, in theory, occupy any area provided for their construction. But can AIRs,
like glaciers, also survive the summer and compound their size every consecutive
winter?

A possible way to study this question is to decrease the air temperature uniformly
(temperature change ∆T ). This will imply a stronger negative sensible heat flux in
summer, thus accelerating icestupa growth and slowing down its decay. We found a
break-even point for ∆T = −2◦ C (Fig. 6.2). For larger negative values of ∆T the
icestupa does not disappear in summer and keeps growing from year to year. For
∆T = −3◦ C, the maximum volume in the fifth year is about 4 times that in the first
year. Therefore, there exists weather conditions where they can last as long as the
water supplies last (see Fig. 6.2). Paper III provides the datasets and methodology
used to produce these simulations.

## Research done so far

My research done so far focussed on estimating the volume evolution of ice stupas and improving their water-use efficiency using software and hardware tools respectively. 

The software tool we developed was an icestupa-specific mass and energy balance model that estimated the quantity of ice, meltwater, sublimation, and wastewater in an hourly resolution. The calibration and validation data basis for this software was the weather, water, and volume measurements carried out with an enormous input of manpower in the Indian Himalayas and the Swiss Alps. In total, measurement datasets of around 25 AIRs across four winters were made available with the support of colleagues from University of Fribourg and Himalayan Institute of Alternatives. Description of datasets associated with 5 AIRs can be found in the published literature.

The AIR software was used to estimate the differing contribution of AIR surface processes built in Guttannen, Switzerland and Ladakh, India. These two locations exhibit different meteorological patterns owing to their significant latitude, longitude and altitude differences. The results revealed that the sublimation process was driving the ice volume differences, and fountain operation of both the AIRs utilized less than one-fifth of the water supply provided. This case study highlighted the importance of colder, drier climates and fountain water supply management when building AIRs with higher volumes and lower water losses.

In response, we developed an automation hardware that could implement fountain scheduling strategies through the AIR software using real-time weather input and location metadata. Simulations converting unscheduled fountains to scheduled fountains improved the water use efficiency of several AIRs more than three fold. Fountain operation using scheduling strategies produced similar ice volumes while consuming one-tenth of the water the unscheduled fountain used. Overall, these results showed that automated fountain water supply management can both increase the water use efficiency of AIRs and reduce their maintenance without compromising on their meltwater production.


---
# References