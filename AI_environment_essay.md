---
title: Maximizing Water Efficiency in AI Datacenters
author: Justin Peabody
date: 11/24/25
abstract: |
 The carbon emissions and energy consumption incurred by data centers, particularly those that use AI, are an area of intense research and innovation. However,insufficient regard is given to these data centers' water use. Many methods have been proposed to reduce the amount of water used for thermoregulation, electricity generation, and computer chip manufacturing. The optimal water efficiency methods vary based on a data center's size and location. In this essay, I explain why more attention should be paid to data center water footprint. Then, I distinguish between the types of water use by data centers and argue for the techniques best suited to reduce each type of water use for data centers located in Chicago. I argue three points: 1) direct-to-chip cooling is the most water efficient and holitically sustainable cooling method for Chicago data centers, 2) solar power is the most water efficient and climatically versatile method of Chicago data center electricity production, and 3) all data centers should purchase semiconductors from companies that make efforts to reduce or offset manufacturing water footprint. 

bibliography: Essay_citations.json
---

## To Readers ##

This is a full draft of my essay, including an introduction, a terminology and key concepts section, three body paragraphs, and a conclusion. I have placed my claim at the end of my key concepts section because that is where I felt it flowed best, but I am unsure if I have buried my claim too deeply in my essay. 

## Introduction ##

To train Open AI's GPT-3 large language model, a precursor to the popular Chat-GPT, 190,000 kWh of energy was used, and 85,000 kg of CO2 emissions were released [@evermanEvaluatingCarbonImpact2023]. 
This is more electricity than is required to power 18 average United States homes for one year [@ElectricityUseHomes2023].
As the development and deployment of large language models, such as GPT-3 and subsequently ChatGPT, increase and scale up, the need for intelligent data centers increases as well.
The article "Data Centre Glossary (Dictionary): Key Definitions & Insights" defines an intelligent data center as "A data centre that leverages AI, machine learning, and IoT devices to enhance operational efficiency and security" [@topp-mugglestoneDataCentreGlossary].
To fulfill these purposes, intelligent data centers require materials for use in construction, cooling and ventilation systems, and electricity to power its operations, among many other resources. 
Scientific researchers are concerned about the myriad environmental impacts incurred by these needs. 


The impacts that have garnered the most attention and investigation include intelligent data centers' many sources of carbon emissions and energy consumption, including those involved in training and refining machine learning models such as GPT-3 [@evermanEvaluatingCarbonImpact2023].
It is less frequently discussed that, in the state of Illinois alone, 4.833 million liters of water (from both data center cooling and generating the electricity to power the data centers) was used by Microsoft to train the GPT-3 model [@liMakingAILess2025].
Data centers' immense water footprints are equally concerning as their carbon and energy footprints. 
However, the very resource that sustains all life on Earth is often overlooked in assessments of AI's environmental impacts.
The article "Making AI less 'Thirsty' provides an overview of the costs of unchecked water consumption by data centers.
"Making AI less 'Thirsty' states,

>"AI's water footprint—many millions of liters of freshwater consumed for cooling the servers and for electricity generation—has largely remained under the radar and keeps escalating. If not properly addressed, AI's water footprint can potentially become a major roadblock to sustainability and create social conflicts, as freshwater resources suitable for human use are extremely limited and unevenly distributed" [@liMakingAILess2025].

Similar concerns are expressed in the article "AI-embedded Data Centres: Promoting Sustainability and Reducing Water Footprint."
"AI-embedded Data Centres" states,

>"The public is becoming more concerned about the increasing carbon effect of artificial intelligence (AI) models, especially large ones like GPT-3 and GPT-4. But nobody has mentioned the enormous and equally important effect that AI models would have on water. Freshwater scarcity has surpassed population growth, decreasing water resources, and ageing water infrastructure as one of the most pressing issues impacting everyone today" [@hiremathAIEmbeddedDataCentres2024]. 

Both of these articles highlight the vast loss of water available for drinking and other everyday uses that could result from failing to consider the water efficiency of a data center's operations. 
For many who lack financial and technological resources to combat water scarcity, such losses could lead to severe dehydration or even death. The lives of such people therefore depend on more efficient use of water in data centers. 
In light of AI's significant and under-emphasized water usage, this essay will explore and compare various methods of reducing AI models' water consumption. 
While I focus on water footprint, I do not consider it in isolation from carbon and energy efficiency, which I acknowledge as equally important components of data centers' overall sustainability. 

## Terminology, conceptual frameworks, and claim ##

This holistic mindset follows from a conceptual framework known as systems thinking.
As the article "Artificial Intelligence and its Carbon Footprint" describes, 

>"A key feature of systems thinking is the insight that complex systems are more than the sum of their parts. This is revealed through the systems lens, which looks at the behavior of the entire system as a whole, relating the components of the system to each other through causal feedback loops. This can reveal previously unobserved and unexpected behavior, meaning that the “something” a system achieves might not be that which was intended by its designers... Essentially, systems thinking is a conceptual shift from seeing how individual causes give rise to behavior... to seeing how systems themselves behave" [@muArtificialIntelligenceIts2025].

Systems thinking is crucial when considering any environmental issue due to the interconnected and interdependent nature of natural systems. This is seen frequently when studying the dependence of natural systems on other natural systems, such as the delicate balance between predator and prey populations. As "Artificial Intelligence and its Carbon Footprint" suggests, the overall concept of systems thinking extends to the interdependence of human-made systems on natural systems. The buildings humans use for living, education, corporate functions, government, and much more are undeniably reliant on water and electricity to maintain them for future human use. No conceivable piece of human-made infrastructure can exist without the use of natural resources, and data centers are no exception. Thus, the operations of a datacenter and available natural resources are inextricably connected and therefore must be considered in tandem to allow both systems to thrive.

"Artificial Intelligence and its Carbon Footprint" offers an additional conceptual framework through which the environmental impacts of data centers, and proposed solutions to mitigate such impacts, can be deliberated upon and weighed against one another. 

This framework consists of six concepts, which the author introduces with respect to efforts to cut carbon emissions of AI data centers [@muArtificialIntelligenceIts2025]. 
However, I believe they can be extended to discussions of any environmental footprint of the data centers, incluing carbon, water, and energy. 
The six concepts, when generalized to any type of environmental footprint, are as follows:

1) Relevance: Does the proposed solution address the primary causes of (insert footprint)? 

2) Effectiveness: does the proposed solution save significant amounts of water/energy/carbon compared to previously implemented practices?

3) Impact: what are the potential long term environmental impacts of the proposed solution (including undesired ones)?

4) Coherence: does the proposed solution align with global climate efforts and the ethical values of justice, transparency, and resource accessibility?  

5) Efficiency: does the proposed solution make optimal use of resources by minimizing waste withot compromising data center performance?

6) Sustainability: will the proposed solution remain effective as data centers increase in size and scale?

While these criterion may seem arbitrarily chosen, I believe they follow naturally from the notion of systems thinking. To best allow data centers to perform adequately without inflicting harm on the environment, methods of decreasing such environmental impacts must cater to the sources most greatly contributing to the harm, as suggested by the principle of relevance. By aiming solutions towards the most singificant sources of resource consumption, greater amounts of resources can be conserved, giving rise to the principle of effectiveness. Systems thinking promotes understanding of ways one resource's saving can influence the consumption of another, an idea explored in this essay. Understanding these efficiency trade-offs can help gauge which solutions are more sustainable in the long run. By being cognizant of resource consumption, data center operations help ensure that adequate resources are available to those in need of them, promoting the principle of resource accessibility that is part of coherence. To ensure resource accessibility, wasted resources must be reduced as a precondition to being made accessible. Thus, systems thinking, coherence, and efficiency logically agree with one another. The consideration of long term environmental impacts is necessary to ensure data centers continue to operate efficiently in the future, which sustainability is predicated on. The criterion set forth in this conceptual framework are therby products of systems thinking. 

To effectively apply both of these conceptual frameworks to the water footprint of AI data centers, one must first understand the main types of water use by datacenters and the types of water footprints incurred by the centers, which "Making AI Less 'Thirsty'" crisply outlines:

>"AI's water usage spans three scopes: onsite water for datacenter cooling (scope 1), offsite water for electricity generation (scope 2), and supply-chain water for server manufacturing (scope 3)" [@liMakingAILess2025]. 

More specifically, Scope 1 water absorbs thermal energy from the computers and servers in a datacenter and either transfers the heat to another medium (such as air) or is released into a nearby body of water (if a body is available). 
Scope 2 water includes any water involved in the manufacturing, transportation, operation, or maintenance of technology used to generate electricity used by the datacenter, such as a solar panel or a hydrogen fuel cell. 
Scope 3 water primarily consists of the water used to manufacture semiconductors-- silicon chips that regulate the flow of electricity throughout a computer. 
Additional, albeit smaller, Scope 3 water sources include the water used to cool and power the semiconductor manufacturing facilities themselves. 


The whopping, aforementioned 4.833 million liters of water used to train GPT-3 in Illinois only accounts for Scope 1 and 2 water use, not Scope 3.
Distinguishing between these three types of water usage allows one to understand how they are related via systems thinking: reductions in one scope of water usage can sometimes lead to increases in other scopes of usage. 
As the article "WATER USAGE EFFECTIVENESS (WUE™): A GREEN GRID DATA CENTER SUSTAINABILITY METRIC" states, 

>"The total water footprint of potential sites should be determined, including water used in energy production. The cooling system design chosen may reduce water use on-site but possibly boost energy use and increase the data center’s total impact on water usage" [@azevedoWATERUSAGEEFFECTIVENESS2011].

Within each scope of water use, there are two distinct water footprints that a datacenter's operations can have. 
The first is water withdrawal footprint, which describes the total amount of water removed from the environment to sustain a process. 
The second is water consumption footprint, which is the amount of withdrawn water that is not returned to the environment [@liMakingAILess2025]. 
This distinction matters because the water consumption footprint directly quantifies the net loss of water from the environment and therefore directly influences how the environment will respond to the loss of water. 
Also, high water consumption footprints can negatively affect communities facing water scarcity if a datacenter is sited in such a community. 
This leads me to my final introductory point: when deliberating which solutions best mitigate the Scope 1, 2, and 3 water footprints of data centers, the most effective and sustainable solutions are dependent on the location of the datacenter. 

As "Making AI Less 'Thirsty'" explains, 

>"Judiciously deciding when and where to train a large AI model can significantly affect the water footprint. Water efficiency exhibits a spatial-temporal diversity—onsite water efficiency changes due to variations of outside weather conditions, and offsite water efficiency changes due to variations of the grid's energy fuel mixes to meet time-varying demands" [@liMakingAILess2025]. 

Due to such geographic discrepancies in climatic conditions and available energy sources, arguing for a single, globally universalizable set of water-efficient solutions for data centers is unrealistic. Instead, this essay considers the solutions that would best reduce each scope of water use by data centers sited in Chicago, Illinois or the surrounding suburbs. 

To reduce their water consumption footprints while simultaneously minimizing other environmental impacts, data centers in Chicago should implement direct-to-chip cooling, using circulated Lake Michigan water, as their primary cooling method, primarily use electricity produced from solar power, and purchase semiconductors from companies that make efforts to reduce or offset manufacturing water footprint. 

## Scope 1 Water Use ##

The method of direct-to-chip server cooling, in tandem with the circulation of Lake Michigan water into and back out of a datacenter, is the most water efficient method of cooling a datacenter in Chicago and is least likely to present unforeseen environmental impacts.
Chicago is located very close to Lake Michigan -- among the largest freshwater bodies in the United States -- and thus has direct access to the lake's freshwater. 
Thus, pumping water from Lake Michigan into a datacenter to be used for cooling would require less energy than it would if the datacenter were located farther away from the lake.
The article "Sustainable Data Centers: Advancing Energy Efficiency and Resource Optimization" describes how data centers can circulate water from a natural body. 

>"The water is circulated through a heat exchanger or directly through cooling coils, where it absorbs heat and then returns to its source or is expelled after releasing the absorbed heat. Data centers located near large lakes or rivers can leverage this technique to reduce cooling costs significantly" [@vaccaroSustainableDataCenters2025].

By containing Lake Michigan water within cooling coils as it circulates through a datacenter and then expelling the water back into the lake, all the water that is withdrawn from the lake is returned to its source, creating zero water consumption footprint. 
This is an additional benefit on top of the method's lower energy footprint.
However, many might argue that this solution is much less water efficient overall than cooling methods that solely use air. 
Indeed, air conditioning methods have zero water withdrawal footprint by definition, while the method of circulating lake water through the datacenter has high withdrawal footprint. 
However, the high water withdrawal efficiency of air conditioning systems comes at the cost of significantly higher energy consumption.

The article “Design of a New Integrated Air-Water Cooling Method to Improve Energy Use in Data Centers" explains the reason for this trade-off.

>"In air-cooled data centers, the energy consumption required to maintain normal equipment operation through cooling systems typically accounts for over 40% of the total energy consumption of the data center. The inefficiency of air-cooling not only limits the development of data centers but also results in significant energy wastage" [@jiaDesignNewIntegrated2024].

This quotation illustrates a tension between energy and water footprints of in-room air cooling systems -- cooling systems that circulate air throughout the entire datacenter.
These cooling systems are more water efficient since they mostly circulate outside air to create a temperature gradient that cools the datacenter. 
However, they are less energy efficient because they must consume higher amounts of energy to circulate large volumes of air in larger data centers. 
For this reason, in room air cooling becomes even more energy-intensive as data centers increase in size.

This efficiency trade-off hearkens back to systems thinking and the importance of considering water footprint in conjunction with other environmental footprints, as air cooling is highly efficient when considering water consumption alone but less efficient when considering water and energy consumption simulatenously. 
Despite this, many will point out that the energy intensivity of in-room CRAC (computer room air conditioning) systems can be reduced, to some degree, by replacing them with in-rack air cooling systems. 
In contrast to in-room cooling systems, in-rack cooling systems circulate cold air to a single row of servers or computers. 
As the article "Sustainable Data Centers: Advancing Energy Efficiency and Resource Optimization" states, 

>"each CRAC unit is dedicated to cooling one row of server racks, minimizing the distance cold air must travel. The cooling units may be mounted among the racks, overhead, or under the floor. This setup enhances cooling precision, reduces energy loss, and eliminates the need for raised floors, making it more versatile for different building designs" [@vaccaroSustainableDataCenters2025].

A CRAC unit that only needs to cool one row of server racks expends less energy to circulate air to the rack by decreasing the distance cold air must travel.
This may lead many to believe that this type of air conditioning unit is the best solution for Chicago's datacenters.
However, even energy-efficient CRAC units like in-rack units have operational limitations. 
As "Sustainable Data Centers: Advancing Energy Efficiency and Resource Optimization" proceeds to explain, 

>"While in-rack air cooling solutions provide effective thermal management for many scenarios, their efficiency can diminish in high-density configurations where heat loads exceed the capacity of air-based systems to dissipate heat effectively. To address these challenges, liquid cooling technologies have emerged as alternative, leveraging the higher thermal conductivity and specific heat capacity of liquids to manage extreme thermal loads efficiently" [@vaccaroSustainableDataCenters2025].

Water is capable of absorbing much more thermal energy than air per unit of temperature increase -- it is said to have a higher specific heat capacity. 
This means the use of water for cooling data center servers allows for more efficient and effective cooling of the warmest server components, which could prevent the shutdown of an entire server rack. 
In this way, liquid cooling is not only more energy efficient than air cooling, it can also enhance the servers' operational performance in regions, such as Chicago, where an ample supply of water is available. 

Even with the increased heat absorption abilities of water compared to air, not all water cooling systems are equally water or energy efficient. 
An instance of this is a device called a cooling tower, which takes in hot water from a data center, expels some of the heat via evaporation of a small portion of the water, and cycles the cooled water back into the datacenter to absorb more heat from servers. 

"Making AI Less 'Thirsty'" explains the water withdrawal and consumption footprint of cooling towers.
"Making AI Less 'Thirsty'" states,

>"...Some water is evaporated (that is, “consumed”) in the cooling tower to dissipate heat into the environment, while the remaining water moves along an open loop to the heat exchanger to further absorb server heat. Additionally, non-evaporated water can be recycled only a few times (typically 3–10 cycles, depending on water quality) before discharge, requiring continuous clean freshwater replenishment to prevent mineral and salt buildup. Thus, to keep the cooling tower working, new water must be constantly added to make up for the evaporated water and discharged water" [@liMakingAILess2025].

This means that if Lake Michigan water were used to cool Chicago data centers via a cooling tower, not all water withdrawn from the lake would return to the lake due to both the evaporation of water from the tower and the need to frequently replenish the water being cycled through the system. 
Regardless of the quality of the water being cycled between the cooling tower and the data center, it would eventually deplete due to evaporation from the cooling tower, creating considerable withdrawal and consumption footprints.
A more water-efficient method that can use water from natural bodies is direct-to-chip server cooling, which delivers water directly to individual servers to ensure adequate heat absorption from each individual component. 
As “Sustainable Data Centers: Advancing Energy Efficiency and Resource Optimization" explains, 

>"Direct-to-Chip Cooling: In this system dielectric fluid commonly water, ethylene glycol, or a combination of the two – is delivered directly to the hottest components, usually the GPU and/or CPU via a cold plate placed directly on the chip. The electric components are never in direct contact with the coolant, which is circulated through channels within the cold plates. The fluid absorbs the heat produced by the device, converts it into vapor, and then condenses it back into liquid" [@vaccaroSustainableDataCenters2025]. 

Direct-to-chip cooling could be implemented as an energy efficient way of circulating Lake Michigan water through a heat exchanger without compromising water efficiency.
Water can flow from Lake Michigan to the datacenter, through cooling coils, then through the channels within server cold plates (where it absorbs heat), then through subsequent cooling coils (where the water can absorb additional heat from the datacenter), and finally through a series of pumps that return the water to the lake. 
Compared to the simple circulation of Lake Michigan water in and out of a datacenter, this solution would have a benefit analogous to in-rack cooling -- increased ability to absorb heat from individual server components. 
This means the circulated water would absorb more heat on each trip through the data center and would thus require less frequent circulation, further reducing the energy consumed by pumping the water.
In addition to this, liquid water's specific heat capacity, which is higher than the specific heat capacity of air, fluctuates only slightly across its range of liquid temperatures [@SpecificHeatCapacity], allowing direct-to-chip cooling to remain effective even during seasons when Lake Michigan surface temperatures are high. 

## Scope 2 Water Use ##

While water use for onsite cooling is a significant contibutor to data centers' water consumption, efforts to promote the centers' overall water efficiency must also address their offsite (Scope 2 and 3) water use.
To most effectively and sustainably reduce their Scope 2 water use, data centers in Chicago should use electricity generated by solar panels as their primary energy source. 
Solar panels, also called photovoltaic cells or PV cells, have minimal to zero water footprint. 
They are much more water-efficient than the second major type of solar power systems, concentrating solar power systems, which use mirrors to reflect and concentrate sunlight onto a structure containing a large volume of water and then use the steam from the heated water to spin a turbine attached to an electric generator [@hernandezEnvironmentalImpactsUtilityscale2014].
The article "Environmental impacts of utility-scale solar energy" quantifies the water footprint of solar panels in comparison to condensed solar power systems.
"Environmental impacts of utility-scale solar energy" states,

>"USSE technologies vary in their water withdrawal (total volume removed from a water source) and consumption (volume of withdrawn water not returned to the source) rates, creating unique tradeoffs. Photovoltaic energy systems have low rates (0.02 m3/megawatt hours [MW h]), consuming water only for panel washing and dust suppression in places where dust deposition is problematic" [@hernandezEnvironmentalImpactsUtilityscale2014]. 

Despite this water efficiency benefit of PV cells, many would be quick to deny solar panels as the most sustainable power source for Chicago's data centers for several reasons, one being the high variability of annual temperatures in Chicago, which affects the performance of the solar panels.
As "Environmental impacts of utility-scale solar energy" states,

>"Photovoltaic technologies use both direct and diffuse light to convert energy from the sun into electricity, but high ambient temperatures reduce panel efficiency almost linearly. Consequently, cool places with high irradiance are the best locations for capturing solar with PV" [@hernandezEnvironmentalImpactsUtilityscale2014].

Indeed, this lack of energy efficiency in high temperatures incontrovertibly places the overall effectiveness of solar panels in question when considered via systems thinking. 
This is a valid concern for Chicago's data centers considering the fact that during the period from 2000 to 2024, Chicago experienced 11 years of average high temperatures at or above 85 degrees in July, according to the National Weather Service [@usdepartmentofcommerceChicagoOHare19912020].
However, measures can be taken to minimize the reductions in panel efficiency resulting from ambient heat.
The article "Solar Panel Life Cycle Costs: What Illinois Property Owners Need to Know" explains methods of minimizing loss of panel efficiency, including efficiency loss related to heat. 
"Solar Panel Life Cycle Costs" states,

>"Summer heat, while beneficial for energy production, can affect panel efficiency if temperatures exceed 85°F. Installing panels with proper ventilation helps mitigate this issue. Fall presents unique challenges with falling leaves and debris, necessitating routine cleaning to prevent coverage that could reduce energy absorption ... today’s solar panels are engineered to handle these local weather conditions with minimal maintenance. Most systems only require bi-annual professional inspections and occasional cleaning to maintain peak performance throughout their lifecycle" [@SolarPanelLife2025]. 

If data centers source their electricity from solar panels with ventilation systems as described in the quotation, high panel efficiency can be ensured even through Chicago's warmer months and heat waves. As an added bonus, "Solar Panel Life Cycle Costs" mentions that natural rainfall is often sufficient to clean solar panels, perhaps eliminating the already small water consumption footprint from panel washing described in "Environmental impacts of utility-scale solar energy."
Nevertheless, many would still object to the use of solar panels to power data centers on the grounds of the embodied carbon, energy, and water footprint of the panels themselves, another valid concern brought about by systems thinking. 

“Environmental Impacts of Utility-Scale Solar Energy" describes the major sources of solar panels' embodied carbon emissions, stating, 

>"Research reveals that, during the whole lifecycle of PV cells, a large amount of carbon gets released. The carbon footprints are generated from the manufacturing process, transportation, and then during their installation. During the rest of their life, carbon emissions can be caused from maintenance and disassembling of the PV cells. Moreover, it is estimated that around 32–82g CO2 per kWh gets emitted from the total lifespan of a [PV system]" [@hernandezEnvironmentalImpactsUtilityscale2014].

As is the case with the impact of temperature on panel efficiency, measures to minimize these sources of embodied carbon are increasingly deployed. 
Modern methods of solar panel manufacturing are becoming increasingly energy and carbon efficient, and the materials used in panel manufacturing, such as aluminum, glass, and silicon, are usually recyclable when a solar panel ceases to operate, according to "Solar Panel Life Cycle Costs" [@SolarPanelLife2025].

The article "How Solar Manufacturers Are Revolutionizing Clean Production Methods" details various innovations in the PV cell manufacturing process, such as variable frequency drives and closed-loop manufactruing systems, which reduce the portion of solar panels' embodied carbon, energy, and water footprint originating from their production and minimize wasted resources.

"How Solar Manufacturers Are Revolutionizing Clean Production Methods" states, 

>"Variable frequency drives (VFDs) have become standard in production lines, allowing motors and pumps to operate at precisely controlled speeds rather than running at full capacity continuously. This smart power management can reduce energy consumption by up to 50% in certain applications. Similarly, regenerative braking systems in conveyor systems capture and reuse energy that would otherwise be lost as heat" [@jackHowSolarManufacturers2025].

>"In modern solar manufacturing facilities, closed-loop manufacturing systems play a crucial role in minimizing water consumption and environmental impact. These systems implement sophisticated water recycling mechanisms that capture, treat, and reuse process water throughout the production cycle. Advanced filtration technologies, including reverse osmosis and deionization systems, ensure that recycled water meets stringent quality requirements for manufacturing processes. This approach typically reduces freshwater consumption by 70-90% compared to traditional manufacturing methods" [@jackHowSolarManufacturers2025].

While "How Solar Manufacturers Are Revolutionizing Clean Production Methods" does not state it, the manufacturing of aluminum for solar panels and other uses is a major contributor to carbon dioxide emissions, generating over one billion metric tons of CO2 annually, according to the article "Carbon emissions in metal manufacturing productivity: A global analysis of aluminium smelting" [@ahmadCarbonEmissionsMetal2025]. Thus, incorporating increasing proportions of recycled materials into solar panels reduces the need for additional aluminum manufacturing, curbing CO2 emissions and reducing the carbon embodied in the solar panel. While some water and energy must be consumed to manufacture solar panels, both closed-loop manufacturing systems and variable frequency drives cut their respective environmental footprints by at least half, which significantly increases solar panels' overall efficiency. 

Despite promising outlook for solar panels' ever-increasing productivity and efficiency, many alternative sources of energy have been touted as optimal solutions for datacenter power generation.
One such source, geothermal energy, possesses a lower water consumption footprint compared to fossil fuels, as does solar energy [@kaczmarczykLifeCycleWater2024]. 
Additionally, geothermal energy is projected to meet 100% of anticipated growth in datacenter power demands in 13 out of the 15 largest data center markets in the United States [@kingPotentialGeothermalEnergy2025], earning it a reputation as a highly scalable electricity generation method. 
Moreover, this source of electricity has already been used to heat and cool residential and commercial buildings in Chicago.

The article "The Potential for Geothermal Energy to Meet Growing Data Center Electricity Demand" further promotes geothermal energy to power data centers by discussing newer geothermal technologies of greater geographic versatility than conventional technologies.

The article states,

>"This note focuses on the use of enhanced geothermal systems (EGS), one type of next-generation geothermal, in which hydraulic fracturing and horizontal drilling techniques are used to create fractures through which fluid can be injected to be warmed by the Earth’s heated rock formations. Because EGS does not require a naturally permeable hydrothermal reservoir like conventional geothermal, it is able to tap into heat across broader swaths of the globe" [@kingPotentialGeothermalEnergy2025].

In arguing for geothermal energy's widening geographic range, the article displays a chart illustrating the percentage of anticipated data center demand growth that would be met by geothermal energy in each of the 15 largest markets in the United States. 

![](https://rhg.com/wp-content/uploads/2025/03/Figure-3-1.png)

The above chart shows that the only two data center markets that would not be entirely accommodated by geothermal energy are Chicago and Washington, D.C. 
Geothermal energy is estimated to accommodate only 46% of Chicago data centers' power needs. All of the markets shown in the chart that would be fully accommodated by geothermal energy are located in the Western United States (Arizona, Nevada, California, Texas, Colorado, and Oregon), while the other two markets are not. 
This suggests that the Western United States has greater available reserves of geothermal energy than the Midwest and East.
Thus, geothermal energy, while useful for heating and cooling buildings, is likely not scalable as the primary source of power for Chicago's data centers due to its relatively limited supply in the Midwest.  

Another electricity production technology, hydrogen fuel cells, are garnering increased attention due to their nonexistent operational carbon and water footprints and low operational energy footprints. 

The article "Hydrogen Fuel Cells in Data Centers: A Clean Energy Revolution" describes how these fuel cells use hydrogen gas to produce electricity, stating,

>"Hydrogen fuel cells are advanced energy systems that convert hydrogen gas into electricity through a chemical reaction with oxygen. This environmentally friendly process produces only water as a byproduct, making it an exceptionally sustainable choice for powering data centers. Unlike intermittent power sources, hydrogen fuel cells provide a reliable and efficient energy supply that is crucial for data centers, ensuring clean and continuous power when needed most" [@saathoffHydrogenFuelCells2024]. 

The very fact that hydrogen fuel cells produce water as a byproduct means that, if such a fuel cell were installed in a data center in Chicago, the water produced by the fuel cell can either supplement water from Lake Michigan for cooling a data center or be piped directly to Lake Michigan, if the water is run through adequate filtration systems first.
In the former case, the fuel cell would have zero water consumption and withdrawal footprints. 
In the latter case, both of these footprints would be negative.
Like solar panels, hydrogen fuel cells are a very clean source of energy at the operational scope, with hydrogen fuel cells being slightly cleaner due to their zero to negative water consumption.
However, examining the embodied footprints of these fuel cells reveals the considerable footprints of the methods used to produce, store and transport hydrogen gas.
“Hydrogen as an Alternative Fuel: A Comprehensive Review of Challenges and Opportunities in Production, Storage, and Transportation" states,

>"The environmental sustainability of hydrogen production is heavily influenced by the methods used to generate it... a significant 62% of global hydrogen production relies on natural gas without carbon capture, utilization, and storage (CCUS), while 21% comes from coal. Only a small portion is produced through electrolysis, a cleaner method that can be powered by renewable energy sources like wind or solar. This heavy dependence on fossil fuels leads to considerable carbon emissions, which challenge hydrogen's potential as a truly clean and sustainable energy carrier" [@hossainbhuiyanHydrogenAlternativeFuel2025].

"Hydrogen as an Alternative Fuel" also explains a multitude of economic difficulties related to hydrogen as an electricity source, stating that hydrogen produced via electrolysis (called green hydrogen) is the most expensive to extract, and the high costs of building and installing devices capable of performing electrolysis is a major barrier to the upscaling of hydrogen fuel for electicity [@hossainbhuiyanHydrogenAlternativeFuel2025]. 

<!-- Discuss wind power here and how it could be combined with hydrogen fuel and/or solar in the near future as an optimal fuel mix for Chicago data centers.-->

Ideally, all hydrogen fuel produced would be green hydrogen, but this is not currently possible due to the energy intensive nature of hydrogen extraction, subsidies to fossil fuels, other aforementioned economic barriers, and a lack of infrastructure for extracting and storing the hydrogen. In contrast, solar energy requires no specialized storage facilities or elaborate extraction technologies. 
Green hydrogen is a theoretically promising solution due to its excellent operational cleanliness. 
If the necessary infrastructure is developed and policies such as carbon taxes are enacted to discourage combustion of fossil fuels, hydrogen fuel cells could become a more sustainable solution than solar panels for powering Chicago's data centers. Until then, however, solar panels appear to be the most holistically efficient and environmentally conscious option, considering aforementioned trends in panel manufacturing procedures.


## Scope 3 Water Use ##

Purchasing semiconductors from companies that strive to decrease their own water consumption is the most effective way and the only way a Chicago data center--or any data center, for the matter -- can reduce their Scope 3 water usage.

The article “Semiconductor Manufacturing and Big Tech’s Water Challenge" quantifies the use of water for semiconductor manufacturing.

>"Ultrapure water, which is thousands of times cleaner than drinking water, is treated through processes such as deionization and reverse osmosis to remove pollutants, minerals and other impurities that can damage chips. It takes roughly 1,400 to 1,600 gallons of municipal water to make 1,000 gallons of ultrapure water... An average chip manufacturing facility today can use 10 million gallons of ultrapure water per day—as much water as is used by 33,000 US households every day" [@jamesSemiconductorManufacturingBig2024].

These statistics emphasize, and place into perspective, the magnitude of the embodied water footprint data centers harbor when semiconductors are purchased to place in their computers. 
This footprint unfortunately cannot be reduced via operational modifications within the data center because it is all incurred offsite. 
The only way this footprint can be reduced is if the manufacturing companies from which data centers purchase the semiconductors make efforts to reduce or offset some of their water withdrawal and consumption footprints. 
Fortunately, there are semiconductor companies that have done so. 
The article "A Spatially Explicit Assessment of Water Use by the Global Semiconductor Industry" mentions one such company, Intel.

>"A large fab manufacturing facility may withdraw 3–5 million gallons per day for feedwater, although at high efficiency facilities like Intel, up to 80% of this will be returned to water bodies" [@frostSpatiallyExplicitAssessment2017].

This quotation implicitly emphasizes that, of the massive amounts of water withdrawn to be converted into ultrapure water for cleaning silicon chips, not all of it is returned to its original source, creating a consumptive water footprint.  
As of the article's publishing in 2017, an estimated 97.26% of Intel's water consumption footprint consisted of water used to manufacture semiconductor chips [@frostSpatiallyExplicitAssessment2017].
Since then, Intel has made massive strides in water withdrawal and consumption footprint reduction, dramtically increasing the percentage of withdrawn water that is returned to water bodies, as explained in Intel's 2024-25 Corporate Responsibility Report.

The report states,

>"In 2024, we returned and restored 106% (by volume) of our fresh water withdrawals to our communities through efficient water management, water reuse, and projects funded by Intel that enabled water restoration in local watersheds...As a part of our 2030 goals, we aim to achieve net positive water by conserving 60 billion gallons of water (cumulative from 2020) and funding projects that will restore more fresh water than we consume to our local watersheds. Our water conservation efforts saved approximately 10.5 billion gallons of water in 2024. Since 2020, our water conservation efforts have saved approximately 46.7 billion gallons of water, enough to sustain about 430,000 US homes for one year" [@IntelCorporateResponsibility]. 

Intel has funded 20 watershed restoration projects in Arizona, three in California, three in New Mexico, one in Ohio, seven in Oregon, one in Texas, two in India, two in Costa Rica, one in Ireland, one in Malaysia, one in Mexico, and one in Vietnam [@IntelCorporateResponsibility]. The company's commitment to increasing the water supply in these watersheds reflects their committment to addressing global water scarcity while simultaneously maintaining viable semiconductor production. By purchasing semiconductors from companies with similar water conservation missions as Intel, data centers financially support practices that prioritize people and the planet as much as profits. This means that even data centers located in regions with little to no water scarcity, such as the city of Chicago, can actively reduce this problem for other regions without sacrificing semiconductor quality by carefully choosing the companies to purchase semiconductors from.

## Conclusion ##

To optimize Scope 1, 2, and 3 water usage while minimally compromising operational performance. energy efficiency, and carbon footprint, data centers in Chicago should use direct-to-chip cooling with Lake Michigan water as their primary cooling method, use electricity produced from solar panels as their main power source, and purchase semiconductors from companies that make efforts to reduce or offset the water used to produce semiconductors. 

In light of the sixfold conceptual framework and the principle of systems thinking, the use of direct-to-chip cooling with Lake Michigan water is the best way for Chicago data centers to reduce their Scope 1 water usage. 
It is relevant by directly addressing the main cause of Scope 1 water footprint in data centers (cooling). 
It is both effective and efficient because it uses water but returns the water to Lake Michigan, making its water consumption footprint zero while reducing the energy footprint compared to air cooling systems and liquid cooling systems that don't use direct-to-chip cooling.
Its long term environmental impacts would be minimal as long as the heat exchangers and cooling coils involved in the cooling process are adequately resistant to corrosion and thus do not contaminate the water circulating through them. 
The return of Lake Michigan water to the source allows Lake Michigan water to remain accessible to Chicagoans and other communities that depend on it, making this solution coherent with the ethical values of resource accessibility and environmental justice.  
The direct delivery of water to individual servers also ensures that adequate cooling occurs on the server level regardless of the size of the data center, making this method a sustainable solution as data centers scale up and increase in size. 
All of these attributes comply with systems thinking because the solution is simultaneously conscious of water and energy use. 

Under the same frameworks, the use of electricity produced by solar panels to power Chicago's data centers is the best way for such data centers to reduce Scope 2 water usage. 
It is relevant by directly addressing the main cause of Scope 2 water footprint in data centers (electricity generation). 
High energy and carbon footprints involved in the manufacturing of solar panels formerly made their use for electricity generation an ineffective and inefficient solution, but as these embodied footprints have drastically decreased in recent decades due to innovations in the panel manufacturing process, PV cells are becoming much more effective and efficient.
As long as measures are taken to ensure the solar panel's sustained panel efficiencies and the maximum recyclability of panel materials, long term environmental impacts of PV cells are minimal.
Formerly, the manufacturing process of solar panels did not align with global climate efforts due to high carbon emissions, but the positive strides being taken in this arena have steered the use of solar panels towards carbon reduction goals, making it an increasingly coherent solution. 
It is possible that, in the near future, Chicago's AI data centers might scale up to the point where solar electricity alone isn't sufficient to power them. 
For this reason, investment into and development of green hydrogen production methods are necessary to eventually transition from solar power to hydrogen fuel cells or a hybrid solar/hydrogen fuel system. 

Finally, to reduce their Scope 3 water use, data centers should purchase semiconductors from manufacturing companies that have water-saving strategies at the forefront of their operations.
This solution's relevance comes from the fact that the majority of such companies' water use originates from the manufacturing process [@jamesSemiconductorManufacturingBig2024], as was formerly the case with the company Intel [@frostSpatiallyExplicitAssessment2017].
Effectiveness and ethical coherence are established via the solutions implemented by the companies, such as water recycling methods and watershed restoration projects. 
Coherence is also established by the reporting of water efficient semiconductor manufacturing processes via corporate sustainability reports, which highlights these companies' commitment to transparency. 
Such companies' commitment to minimizing wasted water, via water recylcing and the use of excess water to restore watersheds, highlights their commitment to efficiency.
Data centers purchasing semiconductors from such companies allows the companies to continue funding water saving efforts, meaning this solution can only have positive long term environmental impacts. 
Additionally, recycling some of the water used to produce a semiconductor allows for additional water to be used to produce more semiconductors, which could allow semiconductor manufacturing facilities to upscale their production in response to increased data center demand, as long as the upscaling does not increase water consumption footprint to the point of watershed depletion.

## Limitations and new implications of my research ##

While I address the carbon and energy footprints associated with the sources of data center water consumption, my emphasis on water footprint omits discussion of many sources of carbon emissions and energy consumption within data centers. 
The solutions argued in this essay do not, and are not intended to, encompass the full repertoire of solutions required to mitigate all aspects of Chicago data centers' overall environmental sustainability. 
They are intended to be a starting point for giving increased consideration towards water footprint, a lesser emphasized aspect of data centers' overall environmental footprint. 
Most notably, I mention, but do not elaborate upon, the carbon emissions and energy consumption associated with training and refining machine learning models. Much research has been done to develop more efficient training algorithms and techniques. For more information about these areas of research, explore these sources:


Everman, Brad, Trevor Villwock, Dayuan Chen, Noe Soto, Oliver Zhang, and Ziliang Zong. 2023. “Evaluating the Carbon Impact of Large Language Models at the Inference Stage.” 2023 IEEE International Performance, Computing, and Communications Conference (IPCCC), November, 150–57. https://doi.org/10.1109/IPCCC59175.2023.10253886.

Ali, Samr, Emmanuel Thepie Fapi, Brigitte Jaumard, and Antoine Planche. 2024. “Focus on Carbon Dioxide Footprint of AI/ML Model Training.” 2024 Intelligent Methods, Systems, and Applications (IMSA), July, 524–29. https://doi.org/10.1109/IMSA61967.2024.10652803.

May, Stow, and Stewart Ashley Ajumoke. 2025. “Reducing Carbon Footprint of Machine Learning Through Model Compression and Pruning.” International Journal of Innovative Science and Research Technology, August 28, 1479–503. https://doi.org/10.38124/ijisrt/25aug970.


This essay focuses on the measures data centers can take to reduce their water footprints at the level of cooling system design, power sources, and semiconductor purchases. 
However, user queries are the ultimately driver of the operation of AI models in data centers, and consequently regulate the amount of water the centers consume. 
Perhaps another part of the solution to mitigating AI's environmetnal footprint is for smaller businesses and individuals to make wiser use of AI, so as not to overly tax the data center servers and reduce the amount of water, energy, and carbon consumed in query processing. 
In light of this, what constitutes "wise" and "unwise" ways for individuals and small businesses to use AI? 

## Bibliography ##























