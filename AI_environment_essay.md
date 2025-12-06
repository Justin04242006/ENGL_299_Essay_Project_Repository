---
title: Maximizing Water Efficiency in AI Datacenters -- A Proposal for the Chicago Region
author: Justin Peabody
date: 12/11/25
abstract: |
 The carbon emissions and energy consumption incurred by data centers, particularly those that use AI, are an area of intense research and innovation. However,insufficient regard is given to these data centers' water use. Many methods have been proposed to reduce the amount of water used for thermoregulation, electricity generation, and computer chip manufacturing. The optimal water efficiency methods vary based on a data center's size and location. In this essay, I explain why more attention should be paid to data center water footprint. Then, I distinguish between the types of water use by data centers and argue for the techniques best suited to reduce each type of water use for data centers located in Chicago. I argue three points: 1) direct-to-chip cooling is the most water efficient and holitically sustainable cooling method for Chicago data centers, 2) solar power is the most water efficient and climatically versatile method of Chicago data center electricity production, and 3) all data centers should purchase semiconductors from companies that make efforts to reduce or offset manufacturing water footprint. 

bibliography: Essay_citations.json
---

## Introduction ##

To train Open AI's GPT-3 large language model, a precursor to the popular Chat-GPT, 190,000 kWh of energy was used, and 85,000 kg of CO2 emissions were released [@evermanEvaluatingCarbonImpact2023]. 
This is more electricity than is required to power 18 average United States homes for one year [@ElectricityUseHomes2023].
As the development and deployment of large language models, such as GPT-3 and subsequently ChatGPT, increase and scale up, the need for intelligent data centers increases as well.
A glossary of key terms in the field of data centers The article "Data Centre Glossary (Dictionary): Key Definitions & Insights" defines an intelligent data center as "A data centre that leverages AI, machine learning, and IoT devices to enhance operational efficiency and security" [@topp-mugglestoneDataCentreGlossary].
To fulfill these purposes, intelligent data centers require materials for use in construction, cooling and ventilation systems, and electricity to power its operations, among many other resources. 
Scientific researchers are concerned about the myriad environmental impacts incurred by these needs. 


The impacts that have garnered the most attention and investigation include intelligent data centers' many sources of carbon emissions and energy consumption, including those involved in training and refining machine learning models such as GPT-3 [@evermanEvaluatingCarbonImpact2023].
It is less frequently discussed that, in the state of Illinois alone, 4.833 million liters of water (from both data center cooling and generating the electricity to power the data centers) was used by Microsoft to train the GPT-3 model [@liMakingAILess2025].
Data centers' immense water footprints are equally concerning as their carbon and energy footprints. 
However, the very resource that sustains all life on Earth is often overlooked in assessments of AI's environmental impacts.

The article "Making AI less 'Thirsty'" explains that the consumption of water by AI data centers, which consists of "many millions of liters of freshwater consumed for cooling the servers and for electricity generation," is "under the radar" with respect to innovation and attention [@liMakingAILess2025]. 
This article also mentions the spatial discrepancy of available water resources, which hints at the issue of water scarcity. 
Water scarcity is explicity voiced as a concern in the article "AI-embedded Data Centres: Promoting Sustainability and Reducing Water Footprint". It expresses similar concerns regarding the lack of recognition of data center water footprints, stating, 
"The public is becoming more concerned about the increasing carbon effect of artificial intelligence (AI) models, especially large ones like GPT-3 and GPT-4. But nobody has mentioned the enormous and equally important effect that AI models would have on water. Freshwater scarcity has surpassed population growth, decreasing water resources, and ageing water infrastructure as one of the most pressing issues impacting everyone today" [@hiremathAIEmbeddedDataCentres2024]. 

Both of these articles highlight the vast loss of water available for drinking and other everyday uses that could result from failing to consider the water efficiency of a data center's operations. 
For many who lack financial and technological resources to combat water scarcity, such losses could lead to severe dehydration or even death. The lives of such people therefore depend on more efficient use of water in data centers. 
In light of AI's significant and under-emphasized water usage, this essay will explore and compare various methods of reducing AI models' water consumption. 
While I focus on water footprint, I do not consider it in isolation from carbon and energy efficiency, which I acknowledge as equally important components of data centers' overall sustainability. 

## Terminology, conceptual frameworks, and claim ##

This holistic mindset follows from a conceptual framework known as systems thinking, which is introduced in the article "Artificial Intelligence and Its Carbon Footprint."

The article "Artificial Intelligence and its Carbon Footprint" describes this framework in the context of the carbon footprints of intelligent data centers, stating,
>A key feature of systems thinking is the insight that complex systems are more than the sum of their parts. This is revealed through the systems lens, which looks at the behavior of the entire system as a whole, relating the components of the system to each other through causal feedback loops. This can reveal previously unobserved and unexpected behavior, meaning that the “something” a system achieves might not be that which was intended by its designers... Essentially, systems thinking is a conceptual shift from seeing how individual causes give rise to behavior... to seeing how systems themselves behave [@muArtificialIntelligenceIts2025].

While this description of systems thinking is used to frame a discussion of carbon footprint reduction, this framework is crucial when considering any environmental issue due to the interconnected and interdependent nature of all natural systems. This is seen frequently when studying the dependence of natural systems on other natural systems, such as the delicate balance between predator and prey populations. As "Artificial Intelligence and its Carbon Footprint" suggests, the overall concept of systems thinking extends to the interdependence of human-made systems on natural systems. The buildings humans use for living, education, corporate functions, government, and much more are undeniably reliant on water and electricity to maintain them for future human use. No conceivable piece of human-made infrastructure can exist without the use of natural resources, and data centers are no exception. Thus, the operations of a datacenter and available natural resources, such as water, are inextricably connected and therefore must be considered in conjunction to allow both systems to thrive. 

"Artificial Intelligence and its Carbon Footprint" offers an additional conceptual framework through which the environmental impacts of data centers, and proposed solutions to mitigate such impacts, can be deliberated upon and weighed against one another. 

This framework consists of six concepts, which the author introduces with respect to efforts to cut carbon emissions of AI data centers [@muArtificialIntelligenceIts2025]. 
However, I believe they can be extended to discussions of any environmental footprint of the data centers, incluing carbon, water, and energy. 
The six concepts, when generalized to any type of environmental footprint, are as follows:

1) Relevance: Does the proposed solution address the primary causes of the footprint? 

2) Effectiveness: does the proposed solution save significant amounts of water/energy/carbon compared to previously implemented practices?

3) Impact: what are the potential long term environmental impacts of the proposed solution, including undesired ones?

4) Coherence: does the proposed solution align with global climate efforts and the ethical values of justice, transparency, and resource accessibility?  

5) Efficiency: does the proposed solution make optimal use of resources by minimizing waste withot compromising data center performance?

6) Sustainability: will the proposed solution remain effective as data centers increase in size and scale?

While these criteria may seem arbitrarily chosen, I believe they follow naturally from the notion of systems thinking. To optimize data center performance without inflicting environmental harm, methods of decreasing such harm must cater to the sources most greatly contributing to it, as suggested by the principle of relevance, the first of the six principles enumerated above. Greater amounts of resources can be conserved if solutions aim towards the predominant sources of resource consumption, giving rise to the principle of effectiveness. Systems thinking promotes understanding of how conserving one resource can increase the consumption of another, an idea explored in this essay. Knowledge of these efficiency trade-offs helps gauge the long term environmental effects of proposed solutions, coinciding with the principle of impact. Awareness of such long term impacts allows data center operations to be tailored to prevent excessive resource consumption now and into the future, promoting resource accessibility under the principle of coherence. To ensure resource accessibility, wasted resources must be reduced as a precondition to being accessible, a key component of the principle of efficiency. Efficient future data center operation, which sustainability is predicated on, requires the consideration of long term environmental impacts. The criterion set forth in this conceptual framework are thus logical extensions of systems thinking. 

To effectively apply both of these conceptual frameworks to the water footprint of AI data centers, one must first understand the main types of water use by datacenters and the types of water footprints incurred by the centers. 
"Making AI Less 'Thirsty'" crisply outlines these usage types, which consist of "onsite water for datacenter cooling (scope 1), offsite water for electricity generation (scope 2), and supply-chain water for server manufacturing (scope 3)" [@liMakingAILess2025]. 

More specifically, Scope 1 water absorbs thermal energy from the computers and servers in a datacenter and either transfers the heat to another medium (such as air) or is released into a nearby body of water (if a body is available). 
Scope 2 water includes any water involved in the manufacturing, transportation, operation, or maintenance of technology used to generate electricity used by the datacenter, such as a solar panel or a hydrogen fuel cell. 
Scope 3 water primarily consists of the water used to manufacture semiconductors -- silicon chips that regulate the flow of electricity throughout a computer. 
Additional, albeit smaller, Scope 3 water sources include the water used to cool and power the semiconductor manufacturing facilities themselves. 


The whopping, aforementioned 4.833 million liters of water used to train GPT-3 in Illinois only accounts for Scope 1 and 2 water use, not Scope 3.
Distinguishing between these three types of water usage allows one to understand how they are related via systems thinking: reductions in one scope of water usage can sometimes lead to increases in other scopes of usage. 
The article "WATER USAGE EFFECTIVENESS (WUE™): A GREEN GRID DATA CENTER SUSTAINABILITY METRIC" describes an example of this: data center cooling systems with smaller Scope 1 water footprints can sometimes be more energy intensive and have higher Scope 2 footprints as a result of their high energy demands [@azevedoWATERUSAGEEFFECTIVENESS2011].

Within each scope of water use, there are two distinct water footprints that a datacenter's operations can have. 
The first is water withdrawal footprint, which describes the total amount of water removed from the environment to sustain a process. 
The second is water consumption footprint, which is the amount of withdrawn water that is not returned to the environment [@liMakingAILess2025]. 
This distinction matters because the water consumption footprint directly quantifies the net loss of water from the environment and therefore directly influences how the environment will respond to the loss of water. 
Also, high water consumption footprints can negatively affect communities facing water scarcity if a data center is sited in such a community. 
This is the reason for the local focus of my argument: when deliberating which solutions best mitigate the Scope 1, 2, and 3 water footprints of data centers, the most effective and sustainable solutions are dependent on the location of the datacenter. 
"Making AI Less 'Thirsty'" explains, "Water efficiency exhibits a spatial-temporal diversity—onsite water efficiency changes due to variations of outside weather conditions, and offsite water efficiency changes due to variations of the grid's energy fuel mixes to meet time-varying demands" [@liMakingAILess2025]. 

Due to such geographic discrepancies in climatic conditions and available energy sources, arguing for a single, globally universalizable set of water-efficient solutions for data centers is unrealistic. Instead, this essay considers the solutions that would best reduce each scope of water use by data centers sited in Chicago, Illinois or the surrounding suburbs. 

To reduce their water consumption footprints while simultaneously minimizing other environmental impacts, data centers in Chicago should implement direct-to-chip cooling, using circulated Lake Michigan water as their primary cooling method, primarily use electricity produced from solar power, and purchase semiconductors from companies that make efforts to reduce or offset manufacturing water footprint. 

## Scope 1 Water Use ##

The method of direct-to-chip server cooling, in tandem with the circulation of Lake Michigan water into and back out of a datacenter, is the most water efficient method of cooling a datacenter in Chicago and is least likely to present unforeseen environmental impacts.
Chicago is located very close to Lake Michigan -- among the largest freshwater bodies in the United States -- and thus has direct access to the lake's freshwater. 
Thus, pumping water from Lake Michigan into a datacenter to be used for cooling would require less energy than it would if the datacenter were located farther away from the lake.
The article "Sustainable Data Centers: Advancing Energy Efficiency and Resource Optimization" describes how data centers can circulate water from a natural body, explaining that the water can be pumped through heat exchanging devices called cooling coils, absorb heat from the data center as it circulates through the coils, and then be returned directly to its source [@vaccaroSustainableDataCenters2025].

By containing Lake Michigan water within cooling coils as it circulates through a datacenter and then expelling the water back into the lake, all the water that is withdrawn from the lake is returned to its source, creating zero water consumption footprint. 
This is an additional benefit on top of the method's lower energy footprint.
However, many might argue that this solution is much less water efficient overall than cooling methods that solely use air. 
Indeed, air conditioning methods have zero water withdrawal footprint by definition, while the method of circulating lake water through the datacenter has high withdrawal footprint. 
However, the high water withdrawal efficiency of air conditioning systems comes at the cost of significantly higher energy consumption.

Researcher Deyi Jia explains the reason for this trade-off, stating, 
"In air-cooled data centers, the energy consumption required to maintain normal equipment operation through cooling systems typically accounts for over 40% of the total energy consumption of the data center. The inefficiency of air-cooling not only limits the development of data centers but also results in significant energy wastage" [@jiaDesignNewIntegrated2024].

This quotation illustrates a tension between energy and water footprints of in-room air cooling systems -- cooling systems that circulate air throughout the entire datacenter.
These cooling systems are more water efficient since they mostly circulate outside air to create a temperature gradient that cools the datacenter. 
However, they are less energy efficient because they must consume higher amounts of energy to circulate large volumes of air in larger data centers. 
For this reason, in room air cooling becomes even more energy-intensive as data centers increase in size.

This efficiency trade-off hearkens back to systems thinking and the importance of considering water footprint in conjunction with other environmental footprints, as air cooling is highly efficient when considering water consumption alone but less efficient when considering water and energy consumption simulatenously. 
Despite this, many will point out that the energy intensivity of in-room CRAC (computer room air conditioning) systems can be reduced, to some degree, by replacing them with in-rack air cooling systems. 
In contrast to in-room cooling systems, in-rack cooling systems circulate cold air to a single row of servers or computers. 
Researcher Viviana Vaccaro explains that in-rack cooling systems "reduce energy loss" and "enhance cooling precision" by "minimizing the distance cold air must travel" [@vaccaroSustainableDataCenters2025].

A CRAC unit that only needs to cool one row of server racks expends less energy to circulate air to the rack by decreasing the distance cold air moves from the cooling unit, which is installed closer to a particular row of server racks.
This may lead many to believe that this type of air conditioning unit is the best solution for Chicago's datacenters.
However, even energy-efficient CRAC units like in-rack units have operational limitations. 
As Vaccaro proceeds to explain, 

>While in-rack air cooling solutions provide effective thermal management for many scenarios, their efficiency can diminish in high-density configurations where heat loads exceed the capacity of air-based systems to dissipate heat effectively. To address these challenges, liquid cooling technologies have emerged as alternative, leveraging the higher thermal conductivity and specific heat capacity of liquids to manage extreme thermal loads efficiently[@vaccaroSustainableDataCenters2025].

Water is capable of absorbing much more thermal energy than air per unit of temperature increase -- it is said to have a higher specific heat capacity. 
This means the use of water for cooling data center servers allows for more efficient and effective cooling of the warmest server components, which could prevent the shutdown of an entire server rack. 
In this way, liquid cooling is not only more energy efficient than air cooling, it can also enhance the servers' operational performance in regions, such as Chicago, where an ample supply of water is available. 

However, even with the increased heat absorption abilities of water compared to air, not all water cooling systems are equally water or energy efficient. 
An instance of this is a device called a cooling tower, which takes in hot water from a data center, expels some of the heat via evaporation of a small portion of the water, and cycles the cooled water back into the datacenter to absorb more heat from servers. 

"Making AI Less 'Thirsty'" describes the operation of a cooling tower and such towers' lack of water efficiency, stating,

>...Some water is evaporated (that is, “consumed”) in the cooling tower to dissipate heat into the environment, while the remaining water moves along an open loop to the heat exchanger to further absorb server heat. Additionally, non-evaporated water can be recycled only a few times (typically 3–10 cycles, depending on water quality) before discharge, requiring continuous clean freshwater replenishment to prevent mineral and salt buildup. Thus, to keep the cooling tower working, new water must be constantly added to make up for the evaporated water and discharged water [@liMakingAILess2025].

This means that if Lake Michigan water were used to cool Chicago data centers via a cooling tower, not all water withdrawn from the lake would return to the lake due to both the evaporation of water from the tower and the need to frequently replenish the water being cycled through the system. 
Regardless of the quality of the water being cycled between the cooling tower and the data center, it would eventually deplete due to evaporation from the cooling tower, creating considerable withdrawal and consumption footprints.
A more water-efficient method that can use water from natural bodies is direct-to-chip server cooling, which delivers water directly to individual servers to ensure adequate heat absorption from each individual component. 
Vaccaro describes direct-to-chip cooling as the direct circulation of a fluid, often water, to components of individual servers most likely to overheat. Water travels through channels in metal plates affixed to the server's electric components, allowing for direct heat transfer from the server to the water without any physical contact between the server and the water [@vaccaroSustainableDataCenters2025]. 

Direct-to-chip cooling could be implemented as an energy efficient way of circulating Lake Michigan water through a heat exchanger without compromising water efficiency.
Water can flow from Lake Michigan to the datacenter, through cooling coils, then through the metal cold plates (where it absorbs heat), then through subsequent cooling coils (where the water can absorb additional heat from the datacenter), and finally through a series of pumps that return the water to the lake. 
Compared to the simple circulation of Lake Michigan water in and out of a datacenter, this solution would have a benefit analogous to in-rack cooling -- increased ability to absorb heat from individual server components. 
This means the circulated water would absorb more heat on each trip through the data center and would thus require less frequent circulation, further reducing the energy consumed by pumping the water.
In addition to this, liquid water's specific heat capacity, which is much higher than the specific heat capacity of air, fluctuates only slightly across its range of liquid temperatures [@SpecificHeatCapacity], allowing direct-to-chip cooling to remain effective even during seasons when Lake Michigan surface temperatures are high. 

## Scope 2 Water Use ##

While water use for onsite cooling is a significant contibutor to data centers' water consumption, efforts to promote the centers' overall water efficiency must also address their offsite (Scope 2 and 3) water use.
To most effectively and sustainably reduce their Scope 2 water use, data centers in Chicago should currently use electricity generated by solar panels as their primary energy source and use electricity generated from a mixture of solar, hydrogen fuel and offshore wind power in the near future. 
Solar panels, also called photovoltaic cells or PV cells, have minimal to zero operational water footprint. 
They are much more water-efficient than the second major type of solar power systems, concentrating solar power (CSP) systems, which use mirrors to reflect and concentrate sunlight onto a structure containing a large volume of water and then use the steam from the heated water to spin a turbine attached to an electric generator [@hernandezEnvironmentalImpactsUtilityscale2014].
Environmental science and ecology researcher R.R. Hernandez quantifies the water footprint of solar panels in comparison to CSP systems, stating, "USSE technologies vary in their water withdrawal (total volume removed from a water source) and consumption (volume of withdrawn water not returned to the source) rates, creating unique tradeoffs. Photovoltaic energy systems have low rates (0.02 m3/megawatt hours [MW h]), consuming water only for panel washing and dust suppression in places where dust deposition is problematic" [@hernandezEnvironmentalImpactsUtilityscale2014]. 

Despite this water efficiency benefit of PV cells, many would be quick to deny solar panels as the most sustainable power source for Chicago's data centers for several reasons, one being the high variability of annual temperatures in Chicago, which affects the performance of the solar panels.
As Hernandez proceeds to explain, high ambient temperatures, solar panel efficiency decreases with exposure to ambient temperatures above 85 degrees F. As a result, Hernandez argues that solar panels are best used in "cool places with high irradiance" [@hernandezEnvironmentalImpactsUtilityscale2014].

Indeed, this lack of energy efficiency in high temperatures incontrovertibly places the overall effectiveness of solar panels in question when considered via systems thinking. 
This is a valid concern for Chicago's data centers considering the fact that during the period from 2000 to 2024, Chicago experienced 11 years of average high temperatures at or above 85 degrees in July, according to the National Weather Service [@usdepartmentofcommerceChicagoOHare19912020].
However, measures can be taken to minimize the reductions in panel efficiency resulting from ambient heat.
The article "Solar Panel Life Cycle Costs: What Illinois Property Owners Need to Know" explains methods of minimizing loss of panel efficiency, including efficiency loss related to heat. 
"Solar Panel Life Cycle Costs" explains that "proper ventilation" helps reduce heat-related losses in panel efficiency. The article also states that engineering of solar panels has improved to minimize the energy and resource costs of leaf and debris removal from the panels to the point where "most systems only require bi-annual professional inspections and occasional cleaning to maintain peak performance throughout their lifecycle" [@SolarPanelLife2025]. 

If data centers source their electricity from solar panels with ventilation systems as described, high panel efficiency can be ensured even through Chicago's warmer months and heat waves. As an added bonus, "Solar Panel Life Cycle Costs" mentions that natural rainfall is often sufficient to clean solar panels, perhaps eliminating the already small water consumption footprint from panel washing described in "Environmental impacts of utility-scale solar energy."
Nevertheless, many would still object to the use of solar panels to power data centers on the grounds of the embodied carbon, energy, and water footprint of the panels themselves, another valid concern brought about by systems thinking. 

Hernandez describes the major sources of solar panels' embodied carbon emissions, stating, 

>Research reveals that, during the whole lifecycle of PV cells, a large amount of carbon gets released. The carbon footprints are generated from the manufacturing process, transportation, and then during their installation. During the rest of their life, carbon emissions can be caused from maintenance and disassembling of the PV cells. Moreover, it is estimated that around 32–82g CO2 per kWh gets emitted from the total lifespan of a [PV system] [@hernandezEnvironmentalImpactsUtilityscale2014].

As is the case with the impact of temperature on panel efficiency, measures to minimize these sources of embodied carbon are increasingly deployed. 
Modern methods of solar panel manufacturing are becoming increasingly energy and carbon efficient, and the materials used in panel manufacturing, such as aluminum, glass, and silicon, are usually recyclable when a solar panel ceases to operate, according to "Solar Panel Life Cycle Costs" [@SolarPanelLife2025].

The article "How Solar Manufacturers Are Revolutionizing Clean Production Methods" details various innovations in the PV cell manufacturing process, such as variable frequency drives and closed-loop manufactruing systems, which reduce the portion of solar panels' embodied carbon, energy, and water footprint originating from their production and minimize wasted resources.

"How Solar Manufacturers Are Revolutionizing Clean Production Methods" describes the purpose of variable frequency drives (VFDs) as devices that use artificial intelligence to regulate the operating speeds of motors and pumps used in panel manufacturing facilities, stating that VFD use "can reduce energy consumption by up to 50% in certain applications" [@jackHowSolarManufacturers2025]. The article also mentions that conveyor belts used in the manufacturing process are increasingly equipped with regenerative braking systems, which "capture and reuse energy that would otherwise be lost as heat" [@jackHowSolarManufacturers2025]. A third method of energy and water efficient solar panel manufacturing discussed in the article is the use of closed loop manufacturing systems, which "implement sophisticated water recycling mechanisms that capture, treat, and reuse process water throughout the production cycle" and reduces freshwater consumption footprint by 70-90% [@jackHowSolarManufacturers2025].

While the aforementioned article does not state it, the manufacturing of aluminum for solar panels and other uses is a major contributor to carbon dioxide emissions, generating over one billion metric tons of CO2 annually, according to researcher Shabbir Ahmad [@ahmadCarbonEmissionsMetal2025]. Thus, incorporating increasing proportions of recycled materials into solar panels reduces the need for additional aluminum manufacturing, curbing CO2 emissions and reducing the carbon embodied in the solar panel. While some water and energy must be consumed to manufacture solar panels, both closed-loop manufacturing systems and variable frequency drives cut their respective environmental footprints by at least half, which significantly increases solar panels' overall efficiency. 

Despite promising outlook for solar panels' ever-increasing productivity and efficiency, many alternative sources of energy have been touted as optimal solutions for datacenter power generation.
One such source, geothermal energy, possesses a lower water consumption footprint compared to fossil fuels, as does solar energy [@kaczmarczykLifeCycleWater2024]. 
Additionally, geothermal energy is projected to meet 100% of anticipated growth in datacenter power demands in 13 out of the 15 largest data center markets in the United States [@kingPotentialGeothermalEnergy2025], earning it a reputation as a highly scalable electricity generation method. 
Moreover, this source of electricity has already been used to heat and cool residential and commercial buildings in Chicago.

The article "The Potential for Geothermal Energy to Meet Growing Data Center Electricity Demand" further promotes geothermal energy to power data centers by discussing newer geothermal technologies of greater geographic versatility than conventional technologies.

The article describes one type of new geothermal technology, enhanced geothermal systems (EGS), which utilizes hydraulic fracturing and horizontal drilling to create openings in the Earth's crust through which high pressure fluids can be injected to be boiled by the heat of Earth's mantle and generate steam, from which the heat can be extracted [@kingPotentialGeothermalEnergy2025]. The article explains that EGS, unlike traditional geothermal technologies, can access energy from rock formations that are not "naturally permeable", allowing EGS systems "to tap into heat across broader swaths of the globe" [@kingPotentialGeothermalEnergy2025]. 

In arguing for geothermal energy's widening geographic range, the article displays a chart, inserted below, illustrating the percentage of anticipated data center demand growth that would be met by geothermal energy in each of the 15 largest markets in the United States. 

![](https://rhg.com/wp-content/uploads/2025/03/Figure-3-1.png)

The above chart shows that the only two data center markets that would not be entirely accommodated by geothermal energy are Chicago and Washington, D.C. 
Geothermal energy is estimated to accommodate only 46% of Chicago data centers' power needs. All of the markets shown in the chart that would be fully accommodated by geothermal energy are located in the Western United States (Arizona, Nevada, California, Texas, Colorado, and Oregon), while the other two markets are not. 
This suggests that the Western United States has greater available reserves of geothermal energy than the Midwest and East.
Thus, geothermal energy, while useful for heating and cooling buildings, is likely not scalable as the primary source of power for Chicago's data centers due to its relatively limited supply in the Midwest.  

Another electricity production technology, hydrogen fuel cells, are garnering increased attention due to their nonexistent operational carbon and water footprints and low operational energy footprints. 

The article "Hydrogen Fuel Cells in Data Centers: A Clean Energy Revolution" describes how these fuel cells use hydrogen gas to produce electricity, stating that hydrogen fuel cells bring hydrogen gas into a chemical reaction with oxygen, producing electricity and water as a byproduct. This article touts hydrogen fuel cells as "an exceptionally sustainable choice for powering data centers" since it can be generated constantly, unlike solar, wind, and other intemittent energy sources [@saathoffHydrogenFuelCells2024].

The very fact that hydrogen fuel cells produce water as a byproduct means that, if such a fuel cell were installed in a data center in Chicago, the water produced by the fuel cell can either supplement water from Lake Michigan for cooling a data center or be piped directly to Lake Michigan, if the water is run through adequate filtration systems first.
In the former case, the fuel cell would have zero water consumption and withdrawal footprints. 
In the latter case, both of these footprints would be negative.
Like solar panels, hydrogen fuel cells are a very clean source of energy at the operational scope, with hydrogen fuel cells being slightly cleaner due to their zero to negative water consumption.
However, examining the embodied footprints of these fuel cells reveals the considerable footprints of the methods used to produce, store and transport hydrogen gas.
Researcher Hossain Bhuiyan quntifies these footprints, stating,

>The environmental sustainability of hydrogen production is heavily influenced by the methods used to generate it... a significant 62% of global hydrogen production relies on natural gas without carbon capture, utilization, and storage (CCUS), while 21% comes from coal. Only a small portion is produced through electrolysis, a cleaner method that can be powered by renewable energy sources like wind or solar. This heavy dependence on fossil fuels leads to considerable carbon emissions, which challenge hydrogen's potential as a truly clean and sustainable energy carrier [@hossainbhuiyanHydrogenAlternativeFuel2025].

Hossain also explains a multitude of economic difficulties related to hydrogen as an electricity source, stating that hydrogen produced via electrolysis (called green hydrogen) is the most expensive to extract, and the high costs of building and installing devices capable of performing electrolysis is a major barrier to the upscaling of hydrogen fuel for electicity [@hossainbhuiyanHydrogenAlternativeFuel2025]. 

<!-- Discuss wind power here and how it could be combined with hydrogen fuel and/or solar in the near future as an optimal fuel mix for Chicago data centers.-->

Ideally, all hydrogen fuel produced would be green hydrogen, but this is not currently possible due to the energy intensive nature of hydrogen extraction, subsidies to fossil fuels, other aforementioned economic barriers, and a lack of infrastructure for extracting and storing the hydrogen. In contrast, solar energy requires no specialized storage facilities or elaborate extraction technologies. 
Green hydrogen is a theoretically promising solution due to its excellent operational cleanliness. 
If the necessary infrastructure is developed and policies such as carbon taxes are enacted to discourage combustion of fossil fuels, hydrogen fuel cells could become a more sustainable solution than solar panels for powering Chicago's data centers. Until then, however, solar panels appear to be the most holistically efficient and environmentally conscious immediately available option, considering aforementioned trends in panel manufacturing procedures.

Offshore wind power is yet another form of renewable energy with the potential to be utilized in the Great Lakes.
There are currently no wind turbines in any of the Great Lakes, meaning offshore wind cannot be used to power Chicago's data centers at the present time.
However, Water policy directors Cora Sutherland and Melissa Scanlan cite analyses from the National Renewable Energy Laboratory (NREL), explaining that "the Great Lakes states have enough offshore wind power potential to provide three times as much electricity as all eight Great Lakes states use currently" [@sutherlandGreatLakesOffshore2025]. 
Specifically, the NREL analysis states that offshore wind has the potential to provide 67% of the electricity used annually by the state of Illinois. This points to the use of offshore wind to generate power for Chicago's data centers in the near future. 
Despite this potential, many technological and economic challenges have delayed the installation of wind turbines in Lake Michigan. 
An article by the NREL explains that offshore wind turbine construction requires materials to be delivered by ocean vessels. Such vessels are too wide to navigate the St. Lawrence Seaway, which connects the Great Lakes to the Atlantic Ocean [@laurieExploringOffshoreWind2023]. Additioanlly, the high prevalence of annual winter ice formaiton in the Great Lakes creates uncertainties in the structural integrity of wind turbines throughout the year. 
Therefore, additoanl research must be done into the structural impacts of ice on wind turbines and the development of narrower vessels that are still capable of trasnporting the materials needed for turbine construction.

In this section, I consider sources of electricity generation in isolation from one another as an analytical method of determining the most water efficient primary electrictiy source for Chicago data centers. In reality, however, most energy grids consist of a mixture of multiple fuel sources. Based on my research, Chicago's ideal power grid should consist of a combination of solar, offshore wind, and green hydrogen generated from the solar and wind in the near future. Economic and technological limitations currently prevent the incorporation of green hydrogen and offshore wind, and such limitations will take time, research, and political shifts to overcome.

## Scope 3 Water Use ##

Purchasing semiconductors from companies that strive to decrease their own water consumption is the most effective way and the only way a Chicago data center--or any data center, for the matter -- can reduce their Scope 3 water usage.

The article “Semiconductor Manufacturing and Big Tech’s Water Challenge" quantifies the use of water for semiconductor manufacturing.

>Ultrapure water, which is thousands of times cleaner than drinking water, is treated through processes such as deionization and reverse osmosis to remove pollutants, minerals and other impurities that can damage chips. It takes roughly 1,400 to 1,600 gallons of municipal water to make 1,000 gallons of ultrapure water... An average chip manufacturing facility today can use 10 million gallons of ultrapure water per day—as much water as is used by 33,000 US households every day [@jamesSemiconductorManufacturingBig2024].

These statistics emphasize, and place into perspective, the magnitude of the embodied water footprint data centers harbor when semiconductors are purchased to place in their computers. 
This footprint unfortunately cannot be reduced via operational modifications within the data center because it is all incurred offsite. 
The only way this footprint can be reduced is if the manufacturing companies from which data centers purchase the semiconductors make efforts to reduce or offset some of their water withdrawal and consumption footprints. 
Fortunately, there are semiconductor companies that have done so. 
Sustainability scientist Kali Frost mentions one such company, Intel, stating that "a large fab manufacturing facility may withdraw 3–5 million gallons per day for feedwater, although at high efficiency facilities like Intel, up to 80% of this will be returned to water bodies" [@frostSpatiallyExplicitAssessment2017].

This quotation implicitly emphasizes that, of the massive amounts of water withdrawn to be converted into ultrapure water for cleaning silicon chips, not all of it is returned to its original source, creating a consumptive water footprint.  
As of the article's publishing in 2017, an estimated 97.26% of Intel's water consumption footprint consisted of water used to manufacture semiconductor chips [@frostSpatiallyExplicitAssessment2017].
Since then, Intel has made massive strides in water withdrawal and consumption footprint reduction, dramtically increasing the percentage of withdrawn water that is returned to water bodies, as explained in Intel's 2024-25 Corporate Responsibility Report.

The report states,

>In 2024, we returned and restored 106% (by volume) of our fresh water withdrawals to our communities through efficient water management, water reuse, and projects funded by Intel that enabled water restoration in local watersheds...As a part of our 2030 goals, we aim to achieve net positive water by conserving 60 billion gallons of water (cumulative from 2020) and funding projects that will restore more fresh water than we consume to our local watersheds. Our water conservation efforts saved approximately 10.5 billion gallons of water in 2024. Since 2020, our water conservation efforts have saved approximately 46.7 billion gallons of water, enough to sustain about 430,000 US homes for one year [@IntelCorporateResponsibility]. 

Intel's greater than 100% water return rate does not mean extra water is being produced by the company; rather, the aforementioned efficient water management and water reuse and systems allows the company to return water to natural bodies that would have otherwise been unreturnable. 
Intel has funded 20 watershed restoration projects in Arizona, three in California, three in New Mexico, one in Ohio, seven in Oregon, one in Texas, two in India, two in Costa Rica, one in Ireland, one in Malaysia, one in Mexico, and one in Vietnam [@IntelCorporateResponsibility]. 
The company's commitment to increasing the water supply in these watersheds reflects their committment to addressing global water scarcity while simultaneously maintaining viable semiconductor production. 
By purchasing semiconductors from companies with similar water conservation missions as Intel, data centers financially support practices that prioritize people and the planet as much as profits. 
This means that even data centers located in regions with little to no water scarcity, such as the city of Chicago, can actively reduce this problem for other regions without sacrificing semiconductor quality by carefully choosing the companies to purchase semiconductors from.

## Conclusion ##

To optimize Scope 1, 2, and 3 water usage while minimally compromising operational performance. energy efficiency, and carbon footprint, data centers in Chicago should use direct-to-chip cooling with Lake Michigan water as their primary cooling method, use electricity produced from solar panels as their main power source, and purchase semiconductors from companies that make efforts to reduce or offset the water used to produce semiconductors. These solutions align with the views of systems thinking and the sixfold conceptual framework. 

In light of these frameworks, the use of direct-to-chip cooling with Lake Michigan water is the best way for Chicago data centers to reduce their Scope 1 water usage. 
It is relevant by directly addressing the main cause of Scope 1 water footprint in data centers (cooling). 
It is both effective and efficient due to its nonexistent water consumption footprint and its reduced energy footprint compared to air cooling systems and other liquid cooling systems.
Long term environmental impacts would be minimal as long as the data center heat exchangers are adequately resistant to corrosion and do not contaminate the water circulating through them. 
The return of Lake Michigan water to its source allows such water to remain accessible to Chicagoans and other communities that depend on it, making this solution coherent with the ethical values of resource accessibility and environmental justice.  
The direct delivery of water to individual servers also ensures that adequate cooling occurs on the server level regardless of the size of the data center, making this method a sustainable solution as data centers scale up. 
All of these attributes comply with systems thinking because the solution is simultaneously conscious of water and energy use. 

Under the same frameworks, the use of electricity produced by solar panels to power Chicago's data centers is the best way for such data centers to reduce Scope 2 water usage. 
It is relevant by addressing electricity generation, the primary source of Scope 2 water footprint in data centers. 
PV cells are becoming much more effective and efficient as their embodied carbon and energy footprints decrease due to innovations in the panel manufacturing process.
As long as measures are taken to ensure PV cells' sustained panel efficiencies and the maximum recyclability of panel materials, long term environmental impacts of PV cells are minimal.
Formerly, the manufacturing process of solar panels did not align with global climate efforts due to high carbon emissions, but the positive strides being taken in this arena have steered the use of solar panels towards carbon reduction goals, making it an increasingly coherent solution. 
It is possible that, in the near future, Chicago's AI data centers might scale up to the point where solar electricity alone isn't sufficient to power them. 
For this reason, investment into and development of green hydrogen production methods are necessary to eventually transition from solar power to hydrogen fuel cells and/or offshore wind power or a hybrid solar/hydrogen/wind fuel system. 

Finally, to reduce their Scope 3 water use, data centers should purchase semiconductors from manufacturing companies that have water-saving strategies at the forefront of their operations.
This solution's relevance comes from the fact that the majority of such companies' water use originates from the manufacturing process [@jamesSemiconductorManufacturingBig2024], as was formerly the case with the company Intel [@frostSpatiallyExplicitAssessment2017].
Effectiveness and ethical coherence are established via the solutions implemented by the companies, such as water recycling methods and watershed restoration projects. 
Coherence is also established by the reporting of water efficient semiconductor manufacturing processes via corporate sustainability reports, which highlights these companies' commitment to transparency. 
Such companies' commitment to minimizing wasted water, via water recylcing and the use of excess water to restore watersheds, highlights their commitment to efficiency.
Data centers purchasing semiconductors from such companies allows the companies to continue funding water saving efforts, meaning this solution can only have positive long term environmental impacts. 
Additionally, recycling some of the water used to produce a semiconductor allows for additional water to be used to produce more semiconductors, which could allow semiconductor manufacturing facilities to upscale their production in response to increased data center demand, as long as water consumption footprint does not increase to the point of watershed depletion.

## Limitations and new implications of my research ##

While I address the carbon and energy footprints associated with the sources of data center water consumption, my emphasis on water footprint omits discussion of many sources of carbon emissions and energy consumption within data centers. 
The solutions argued in this essay do not, and are not intended to, encompass the full repertoire of solutions required to mitigate all aspects of Chicago data centers' overall environmental sustainability. 
They are intended to be a starting point for giving increased consideration towards water footprint, a lesser emphasized aspect of data centers' overall environmental footprint. 
Most notably, I mention, but do not elaborate upon, the carbon emissions and energy consumption associated with training and refining machine learning models. Much research has been done to develop more efficient training algorithms and techniques. For more information about these areas of research, explore these sources:

[@aliFocusCarbonDioxide2024]

[@evermanEvaluatingCarbonImpact2023]

[@mayReducingCarbonFootprint2025]

Additionally, I do not consider the adverse ecological effects of the heat return involved in the ciruclation of Lake Michigan water to cool Chicago data centers.
Considering previous discussion of water's high specific heat capacity (water requires very large amounts of heat to raise its temperature), I could speculate that ecological effects might be less than they would if data center heat was simply released into the air. 
However, such speculation would fail to account for the decrease in dissolved oxygen content of warmer water due to algal blooms, which can suffocate aquatic life [@UnderstandingImpactWarming2024]. 
To help reduce such ecological effects, methods of direct to chip cooling that utilize the high specific heat capacity of water, without transferring so much thermal energy to the water that its temperature rises significantly, should be explored. 
This might also necessitate the development of more energy-efficient server components that generate less heat in the first place. 

This essay focuses on the measures data centers can take to reduce their water footprints at the level of cooling system design, power sources, and semiconductor purchases. 
However, user queries are the ultimately driver of the operation of AI models in data centers, and consequently regulate the amount of water the centers consume. 
Perhaps another part of the solution to mitigating AI's environmetnal footprint is for businesses and individuals to make wiser use of AI, so as not to overly tax the data center servers and reduce the amount of water, energy, and carbon consumed in query processing. 

## Bibliography ##























