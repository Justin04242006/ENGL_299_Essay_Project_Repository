#Essay Draft#

###Introduction###

To train Open AI's GPT-3 large language model, a precursor to the popular Chat-GPT, 190,000 kWh of energy was used, and 85,000 kg of CO2 emissions were released (Everman et al. 2023). 
This is more electricity than is required to power 18 average United States homes for one year (“Electricity Use in Homes - U.S. Energy Information Administration (EIA),” n.d.). 
As the development and deployment of large language models, such as GPT-3 and subsequently ChatGPT, increase and scale up, the need for intelligent data centers -- increases as well.
The article "Data Centre Glossary (Dictionary): Key Definitions & Insights" defines an intelligent data center as "A data centre that leverages AI, machine learning, and IoT devices to enhance operational efficiency and security."
To fulfill these purposes, intelligent data centers require materials for use in construction, cooling and ventilation systems, and electricity to power its operations, among many other resources. 
Scientific researchers are concerned about the myriad environmental impacts incurred by these needs. 
The impacts that have garnered the most attention and investigation include intelligent data centers' many sources of carbon emissions and energy consumption, including those involved in training and refining machine learning models such as GPT-3 (Everman et al. 2023). 
It is perhaps less discussed that, in the state of Illinois alone, 4.833 million liters of water (from both data center cooling and generating the electricity to power the data centers) was used by Microsoft to train the GPT-3 model (Li et al. 2025). 
The immense water footprint of data centers is equally concerning as their carbon and energy footprints. 
However, the very resource that sustains all life on Earth is often overlooked in assessments of AI's environmental impacts.

As explained by computer science PhD student Pengfei Li and computer engineering assistant professors Mohammad Atiqul Islam, Jianyi Yang, and Shaolei Ren in the article "Making AI less 'Thirsty'",

>"AI's water footprint—many millions of liters of freshwater consumed for cooling the servers and for electricity generation—has largely remained under the radar and keeps escalating. If not properly addressed, AI's water footprint can potentially become a major roadblock to sustainability and create social conflicts, as freshwater resources suitable for human use are extremely limited and unevenly distributed" (Li et al. 2025).

Associate professor Rahul Hiremath expresses similar concerns in the article "AI-embedded data Centres: Promoting Sustainability and Reducing Water Footprint".
Hiremath states,
"The public is becoming more concerned about the increasing carbon effect of artificial intelligence (AI) models, especially large ones like GPT-3 and GPT-4. But nobody has mentioned the enormous and equally important effect that AI models would have on water. Freshwater scarcity has surpassed population growth, decreasing water resources, and ageing water infrastructure as one of the most pressing issues impacting everyone today" (Hiremath 2024). 

Both of these articles highlight the vast loss of water available for drinking and other everyday uses that could result from failing to consider the water efficiency of a data center's operations. For many who lack financial and technological resources to combat water scarcity, such losses could lead to severe dehydration or even death. The lives of such people therefore depend on smarter use of water in data centers. 

#Terminology and conceptual frameworks#

In light of AI's significant and under-emphasized water usage, this essay will explore and compare various methods of reducing AI models' water consumption. 
While I focus on water footprint, I do not consider it in isolation from carbon and energy efficiency, which I acknowledge as equally important components of data centers' overall sustainability. 
This holistic mindset follows from a broad conceptual framework known as systems thinking.
As the article "Artificial Intelligence and its Carbon Footprint" describes, 

>"A key feature of systems thinking is the insight that complex systems are more than the sum of their parts. This is revealed through the systems lens, which looks at the behavior of the entire system as a whole, relating the components of the system to each other through causal feedback loops. This can reveal previously unobserved and unexpected behavior, meaning that the “something” a system achieves might not be that which was intended by its designers... Essentially, systems thinking is a conceptual shift from seeing how individual causes give rise to behavior... to seeing how systems themselves behave" (Mu et al. 2025)."

Systems thinking is crucial when considering any environmental issue due to the interconnected and interdependent nature of natural systems. This is seen frequently when studying the dependence of natural systems on other natural systems; such as the dependence of predatory fish on a steady supply of prey fish and appropriate temperature and pH levels in the surrounding water. As this quotation suggests, the overall concept extends to the interdependence of human-made systems on natural systems. The buildings humans use for living, education, corporate functions, government, and much more are undeniably reliant on water and electricity to maintain them for future human use. No conceivable piece of human-made infrastructure can exist without the use of natural resources, and data centers are no exception. Thus, the operations of a datacenter and avaialble natural resources are dependent on one another and therefore must be considered in tandem to allow both systems to thrive.

"Artificial Intelligence and its Carbon Footprint" offers an additional conceptual framework through which the environmental impacts of data centers, and proposed solutions to mitigate such impacts, can be deliberated upon. 

This framework consists of six concepts, which the author introduces with respect to efforts to cut carbon emissions of AI data centers (Mu et al. 2025). 
However, I believe they can be extended to discussions of any environmental footprint of the data centers, incluing carbon, water, and energy. 
The six concepts, when generalized to any type of environmental footprint, are as follows:

1) Relevance: Does the proposed solution address the primary causes of (insert footprint)? 

2) Effectiveness: does the proposed solution save significant amounts of water/energy/carbon compared to previously implemented practices?

3) Impact: what are the potential long term environmental impacts of the proposed solution (including undesired ones)?

4) Coherence: does the proposed solution align with global climate efforts and the ethical values of justice, transparency, and resource accessibility?  

5) Efficiency: does (proposed solution) make optimal use of resources by minimizing wasted resources withot compromising data center performance?

6) Sustainability: will (proposed solution) remain effective as data centers increase in size and scale?

While these criterion may seem arbitrarily chosen, I believe they follow naturally from the notion of systems thinking. To best allow data centers to perform adequatelty without inflicting harm on the environment, methods of decreasing such environmental impacts must cater to the sources most greatly contributing to the harm, as suggested by the principle of relevance. By aiming solutions towards the most singificant sources of resource consumption, greater amounts of resources can be saved, giving rise to the principle of effectiveness. Systems thinking promotes understanding of ways one resource's saving can influence the consumption of another, an idea explored in this essay. Understanding these efficiency trade-offs can help gauge which solutions are more sustainable in the long run. By being cognizant of resource consumption, data center operations help ensure that adequate resources are available to those in need of them, promoting the principle of resource accessibility that is part of coherence. To ensure resource accessibility, wasted resources must be reduced as a precondition to being made accessible. Thus, systems thinking, coherence, and efficiency logically agree with one another. The consideration of long term environmental impacts is necessary to ensure data centers continue to operate efficiently in the future, which sustainability is predicated on. Thus, the criterion set forth in this conceptual framework are products of systems thinking. 

To effectively put both of these conceptual frameworks in action when discussing the water footprint of AI data centers, one must first understand the main types of water use by datacenters and the types of water footprints incurred by the centers. 
Water usage by AI datacenters can be divided into three categories.
The article "Making AI Less Thirsty" crisply outlines these categories:

>"AI's water usage spans three scopes: onsite water for datacenter cooling (scope 1), offsite water for electricity generation (scope 2), and supply-chain water for server manufacturing (scope 3)" (Li et al. 2025). 

More specifically, Scope 1 water absorbs thermal energy from the computers and servers in a datacenter and either transfers the heat to another medium (such as air) or is released into a nearby body of water (if a body is available). 
Scope 2 water includes any water involved in the manufacturing, transportation, operation, or maintenance of technology used to generate electricity used by the datacenter, such as a solar panel or a hydrogen fuel cell. 
Scope 3 water primarily consists of the water used to manufacture semiconductors-- silicon chips that regulate the flow of electricity throughout a computer. 
Additional, albeit smaller, Scope 3 water sources include the water used to cool and power the semiconductor manufacturing facilities themselves. 
The whopping, aforementioned 4.833 million liters of water used to train GPT-3 in Illinois only includes Scope 1 and 2 water use, not Scope 3.
Distinguishing between these three types of water usage allows one to understand how they are related via systems thinking: reductions in one scope of water usage can sometimes lead to increases in other scopes of usage. 
As the article "WATER USAGE EFFECTIVENESS (WUE™): A GREEN GRID DATA CENTER SUSTAINABILITY METRIC" states, "The total water footprint of potential sites should be determined, including water used in energy production. The cooling system design chosen may reduce water use on-site but possibly boost energy use and increase the data center’s total impact on water usage" (Azevedo et al. 2011). 
Within each scope of water use, there are two distinct water footprints that a datacenter's operations can have. 
The first is water withdrawal footprint, which describes the total amount of water removed from the environment to sustain the process. 
The second is water consumption footprint, which is the amount of withdrawn water that is not returned to the environment (Li et al. 2025). 
This distinction matters because the water consumption footprint directly quantifies the net loss of water from the environment and therefore directly influences how the environment will respond to the loss of water. 
Also, high water consumption footprints can negatively affect communities facing water scarcity if a datacenter is sited in such a community. 
This leads me to my final introductory point: when deliberating which solutions best mitigate the Scope 1, 2, and 3 water footprints of data centers, the most effective and sustainable solutions change based on the location of the datacenter. 

As "Making AI Less 'Thirsty'" explains, 

>"Judiciously deciding when and where to train a large AI model can significantly affect the water footprint. Water efficiency exhibits a spatial-temporal diversity—onsite water efficiency changes due to variations of outside weather conditions, and offsite water efficiency changes due to variations of the grid's energy fuel mixes to meet time-varying demands" (Li et al. 2025). 

Due to such geographic discrepancies in climatic conditions and available energy sources, arguing for a single, globally universalizable set of water-efficient solutions for data centers is both unrealistic and ignorant of the dependence of the datacenter on the environmental aspects of its location. Instead, this essay will consider the solutions that would be best for data centers sited in Chicago, Illinois or the surrounding suburbs. 

To reduce their water footprints while simultaneously minimizing other environmental impacts, data centers in Chicago should circulate Lake Michigan water, using a technique called direct-to-chip cooling, as their primary cooling method, use electricity produced from solar power as their primary source of electricity, and purchase semiconductors from companies that make efforts to reduce or offset manufacturing water footprint.

#Scope 1 Water Use#

The method of direct-to-chip server cooling, in tandem with the circulation of Lake Michigan water into and back out of a datacenter, is the most water efficient method of cooling a datacenter in Chicago and is least likely to present unforeseen environmental impacts.
Chicago is located very close to Lake Michigan -- among the largest freshwater bodies in the United States -- and thus has direct access to the lake's freshwater. 
Thus, pumping water from Lake Michigan into a datacenter to be used for cooling would require less energy than it would if the datacenter were located farther away from the lake.
The article "Sustainable Data Centers: Advancing Energy Efficiency and Resource Optimization" describes this notion of ciruclation from a natural body of water.
>"The water is circulated through a heat exchanger or directly through cooling coils, where it absorbs heat and then returns to its source or is expelled after releasing the absorbed heat. Data centers located near large lakes or rivers can leverage this technique to reduce cooling costs significantly" (Vaccaro et al. 2025). 
By containing Lake Michigan water within cooling coils as it circulates through a datacenter and then expelling the water back into the lake, all the water that is withdrawn from the lake is returned to its source, creating zero water consumption footprint. 
This is an additional benefit on top of the method's lower energy footprint.
However, many might argue that this solution is much less water efficient overall than cooling methods that solely use air. 
Indeed, air conditioning methods, by definition, have zero water withdrawal footprint, while the method of circulating lake water through the datacenter has high withdrawal footprint. 
However, the high water withdrawal efficiency of air conditioning systems comes at the cost of significantly higher energy consumption.
As the article "“Design of a New Integrated Air-Water Cooling Method to Improve Energy Use in Data Centers" explains, 
>"In air-cooled data centers, the energy consumption required to maintain normal equipment operation through cooling systems typically accounts for over 40% of the total energy consumption of the data center. The inefficiency of air-cooling not only limits the development of data centers but also results in significant energy wastage" (Jia et al. 2024). 
This quotation illustrates a tension between energy and water footprints of in-room air cooling systems -- cooling systems that circulate air throughout the entire datacenter -- which are more water efficient since they mostly circulate outside air to create a temperature gradient that cools the datacenter. 
However, these air cooling systems are less energy efficient because they must consume higher amounts of energy to circulate large volumes of air in larger data centers. 
For this reason, in room air cooling becomes even more energy-intensive as data centers increase in size.
This hearkens back to systems thinking and the importance of considering water footprint in conjunction with other environmental footprints, as air cooling is highly efficient when considering water consumption alone but less efficient when considering water and energy consumption simulatenously. 
Despite this, many will point out that the energy intensivity of in-room CRAC (computer room air conditioning) systems can be reduced, to some degree, by replacing them with in-rack cooling systems. 
In contrast to in-room cooling systems, in-rack cooling systems circulate cold air to a single row of servers or computers. 
As the article "Sustainable Data Centers: Advancing Energy Efficiency and Resource Optimization" states, 

>"each CRAC unit is dedicated to cooling one row of server racks, minimizing the distance cold air must travel. The cooling units may be mounted among the racks, overhead, or under the floor. This setup enhances cooling precision, reduces energy loss, and eliminates the need for raised floors, making it more versatile for different building designs" (Vaccaro et al. 2025). 

A CRAC unit that only needs to cool one row of server racks expends less energy to circulate air to the rack by decreasing the distance cold air must travel.
This may lead many to believe that this type of air conditioning unit is the best solution for Chicago's datacenters.
However, even energy-efficient CRAC units like in-rack units have operational limitations. 
As "Sustainable Data Centers: Advancing Energy Efficiency and Resource Optimization" proceeds to explain, 

>"While in-rack air cooling solutions provide effective thermal management for many scenarios, their efficiency can diminish in high-density configurations where heat loads exceed the capacity of air-based systems to dissipate heat effectively. To address these challenges, liquid cooling technologies have emerged as alternative, leveraging the higher thermal conductivity and specific heat capacity of liquids to manage extreme thermal loads efficiently" (Vaccaro et al. 2025). 

Water is capable of absorbing much more thermal energy than air per unit of temperature increase -- it is said to have a higher specific heat capacity. 
This means the use of water for cooling data center servers allows for more efficient and effective cooling of the warmest server components, which could prevent the shutdown of an entire server rack. 
In this way, liquid cooling is not only more energy efficient than air cooling, it can also enhance the servers' operational performance in regions, such as Chicago, where an ample supply of water is available. 

Even with the increased heat absorption abilities of water compared to air, not all water cooling systems are equally water or energy efficient. 
An instance of this is a device called a cooling tower, which takes in hot water from a data center, expels some of the heat via evaporation of a small portion of the water, and cycles the cooled water back into the datacenter to absorb more heat from servers. 
As "Making AI Less 'Thirsty'" states,

>"...Some water is evaporated (that is, “consumed”) in the cooling tower to dissipate heat into the environment, while the remaining water moves along an open loop to the heat exchanger to further absorb server heat. Additionally, non-evaporated water can be recycled only a few times (typically 3–10 cycles, depending on water quality) before discharge, requiring continuous clean freshwater replenishment to prevent mineral and salt buildup. Thus, to keep the cooling tower working, new water must be constantly added to make up for the evaporated water and discharged water" (Li et al. 2025). 

This means that if Lake Michigan water were used to cool Chicago data centers via a cooling tower, not all water withdrawn from the lake would return to the lake due to both the evaporation of water from the tower and the need to frequently replenish the water being cycled through he system. 
Regardless of the quality of the water being cycled between the cooling tower and the data center, it would eventually deplete due to evaporation from the cooling tower.
Thus, cooling towers are not very water efficient. 
A more water-efficient method that can use Lake Michigan water is direct-to-chip server cooling, which delivers water directly to individual servers to ensure adequate heat absorption from each individual component. 
As “Sustainable Data Centers: Advancing Energy Efficiency and Resource Optimization" explains, 

>"Direct-to-Chip Cooling: In this system dielectric fluid commonly water, ethylene glycol, or a combination of the two – is delivered directly to the hottest components, usually the GPU and/or CPU via a cold plate placed directly on the chip. The electric components are never in direct contact with the coolant, which is circulated through channels within the cold plates. The fluid absorbs the heat produced by the device, converts it into vapor, and then condenses it back into liquid" (Vaccaro et al. 2025). 

This could be implemented as a more energy efficient variation of the circulation of Lake Michigan water through a heat exchanger without compromising the water efficiency of the solution in the note "Circulation of Lake Michigan Water." 
By installing coils that connect to the cold plates on top of chips, water can flow from Lake Michigan to the datacenter, through the coils, then through the channels within the cold plate (where it absorbs heat), then through subsequent cooling coils (where the water can absorb additional heat from the datacenter), and finally through a series of pumps that return the water to the lake. 
Compared to the simple circulation of Lake Michigan water in and out of a datacenter, this solution would have a benefit analogous to in-rack cooling -- increased ability to absorb heat from individual server components. 
This means the ciruclated water would absorb more heat on each trip through the data center and would thus require less frequent pumping, reducing energy consumption. 
In addition to this, liquid water's higher specific heat capacity decreases only slightly across its range of liquid temperatures, allowing this method to remain effective even during seasons with high lake surface temperatures. 

#Scope 2 Water Use#

To most effectively and sustainably reduce their Scope 2 water use, data centers in Chicago should use electricity from photovoltaic cells (solar panels) as their primary energy source. 
Photovoltaic cells have minimal water footprint, if any. 
They are much more water-efficient than the second major type of solar power systems, condensed solar power systems, which involve the use of mirrors to reflect water onto a structure containing a large volume of water and using the steam from the heated water to turn a turbine attached to an electric generator (Hernandez et al. 2014).
As the article "Environmental impacts of utility-scale solar energy" states,
>"USSE technologies vary in their water withdrawal (total volume removed from a water source) and consumption (volume of withdrawn water not returned to the source) rates, creating unique tradeoffs. Photovoltaic energy systems have low rates (0.02 m3/megawatt hours [MW h]), consuming water only for panel washing and dust suppression in places where dust deposition is problematic" (Hernandez et al. 2014).

<!--Supply some analysis here, explaining what a USSE technology is (utility-scale solar energy).-->

Despite this benefit, many would be quick to deny solar panels as the most sustainable power source for Chicago's data centers for several reasons, one being the high variability of annual temperatures in Chicago, which affects the performance of the solar panels.
As "Environmental impacts of utility-scale solar energy" states,

>"Photovoltaic technologies use both direct and diffuse light to convert energy from the sun into electricity, but high ambient temperatures reduce panel efficiency almost linearly ([Fig. 4](https://www.sciencedirect.com/science/article/pii/S1364032113005819#f0020)). Consequently, cool places with high irradiance are the best locations for capturing solar with PV" (Hernandez et al. 2014).

Indeed, this lack of energy efficiency incontrovertibly places the overall sustainability of solar panels in question through the lens of systems thinking. 
This is emphasized considering the fact that, over the past 25 years in Chicago, 5 months of the year have experienced average high temperatures above 85 degrees, according to the National Weather Service (US Department of Commerce, n.d.). 
However, measures can be taken to minimize the reductions in panel efficiency that come with high temperatures.
As the article "Solar Panel Life Cycle Costs: What Illinois Property Owners Need to Know" states, 

>"Summer heat, while beneficial for energy production, can affect panel efficiency if temperatures exceed 85°F. Installing panels with proper ventilation helps mitigate this issue. Fall presents unique challenges with falling leaves and debris, necessitating routine cleaning to prevent coverage that could reduce energy absorption ... today’s solar panels are engineered to handle these local weather conditions with minimal maintenance. Most systems only require bi-annual professional inspections and occasional cleaning to maintain peak performance throughout their lifecycle" (david 2025).

If data centers source their electricity from solar panels with ventilation systems as described in the quotation, high panel efficiency can be ensured even through Chicago's warmer months and heat waves. 

Even so, many would still object to the use of solar panels to power data centers on the grounds of the high embodied carbon footprint of the panels themselves, which a systems thinking mindset should take into account.

 “Environmental Impacts of Utility-Scale Solar Energy" states,

>"Research reveals that, during the whole lifecycle of PV cells, a large amount of carbon gets released. The carbon footprints are generated from the manufacturing process, transportation, and then during their installation. During the rest of their life, carbon emissions can be caused from maintenance and disassembling of the PV cells. Moreover, it is estimated that around 32–82g CO2 per kWh gets emitted from the total lifespan of a [PV system]" (Rahman et al. 2022).

Just like with the impact of temperatures on panel efficiency, measures are being taken to minimize these sources of embodied carbon. 
Modern methods of solar panel manufacturing are becoming increasingly energy and carbon efficient, and the materials used in panel manufacturing, such as aluminum, glass, and silicon, are usually recyclable when a solar panel ceases to operate (david 2025).

<!--Below are quotations from the article "How Solar Manufacturers Are Revolutionizing Clean Production Methods" that explain ways in which solar panel manufacturing processes are becoming more energy, water, and carbon efficient. Supplement them with your own analysis, of course, and paraphrase some as needed to avoid this section feeling too quote-heavy.-->


>"Variable frequency drives (VFDs) have become standard in production lines, allowing motors and pumps to operate at precisely controlled speeds rather than running at full capacity continuously. This smart power management can reduce energy consumption by up to 50% in certain applications. Similarly, regenerative braking systems in conveyor systems capture and reuse energy that would otherwise be lost as heat" (jack. 2025. “How Solar Manufacturers Are Revolutionizing Clean Production Methods.” _Mose Solar_, May 3. [https://www.moserbaersolar.com/uncategorized/how-solar-manufacturers-are-revolutionizing-clean-production-methods/](https://www.moserbaersolar.com/uncategorized/how-solar-manufacturers-are-revolutionizing-clean-production-methods/).)

>"In modern solar manufacturing facilities, closed-loop manufacturing systems play a crucial role in minimizing water consumption and environmental impact. These systems implement sophisticated water recycling mechanisms that capture, treat, and reuse process water throughout the production cycle. Advanced filtration technologies, including reverse osmosis and deionization systems, ensure that recycled water meets stringent quality requirements for manufacturing processes. This approach typically reduces freshwater consumption by 70-90% compared to traditional manufacturing methods" (jack. 2025. “How Solar Manufacturers Are Revolutionizing Clean Production Methods.” _Mose Solar_, May 3. [https://www.moserbaersolar.com/uncategorized/how-solar-manufacturers-are-revolutionizing-clean-production-methods/](https://www.moserbaersolar.com/uncategorized/how-solar-manufacturers-are-revolutionizing-clean-production-methods/).)

>"Aluminum frames, which constitute approximately 12% of a typical solar panel’s mass, are increasingly manufactured using recycled content. Major producers have achieved recycled content rates of 60-80% in their frame components, demonstrating the industry’s commitment to circular economy principles" (jack. 2025. “How Solar Manufacturers Are Revolutionizing Clean Production Methods.” _Mose Solar_, May 3. [https://www.moserbaersolar.com/uncategorized/how-solar-manufacturers-are-revolutionizing-clean-production-methods/](https://www.moserbaersolar.com/uncategorized/how-solar-manufacturers-are-revolutionizing-clean-production-methods/).)

Geothermal energy has been touted as a promising solution for datacenter power generation due to its lower water consumption footprint compared to fossil fuels (Kaczmarczyk et al. 2024) and its ability to meet 100% of anticipated growth in datacenter power demands in 13 out of the 15 largest data center markets in the United States (King et al. 2025). 
Additionally, geothermal energy has promise to be very effective for heating and cooling residential and commercial buildings in Chicago (ABC7 Chicago 2024). 
The article "The Potential for Geothermal Energy to Meet Growing Data Center Electricity Demand" further promotes geothermal energy to power data centers by discussing newer geothermal technologies of greater geographic versatility. 
The article states,

>"This note focuses on the use of enhanced geothermal systems (EGS), one type of next-generation geothermal, in which hydraulic fracturing and horizontal drilling techniques are used to create fractures through which fluid can be injected to be warmed by the Earth’s heated rock formations. Because EGS does not require a naturally permeable hydrothermal reservoir like conventional geothermal, it is able to tap into heat across broader swaths of the globe" (King et al. 2025).

In arguing for geothermal energy's widening geographic range, the article displays a chart showing the percentage of anticipated data center demand growth that would be met by geothermal energy in each of the 15 largest markets in the United States. 
The only two data center markets that would not be entirely accommodated by geothermal energy are Chicago and Washington, D.C. 
Geothermal energy is estimated to accommodate only 46% of Chicago data centers' power needs. All of the markets shown in the chart that would be fully accommodated by geothermal energy are located in the Western United States (Arizona, Nevada, California, Texas, Colorado, and Oregon), while the other two markets are not. 
This means that the Western United States likely has greater available reserves of geothermal energy than the Midwest and East. \
Thus, geothermal energy is not scalable as the primary source of power for Chicago's data centers. 
A newer technology, hydrogen fuel cells are garnering increased attention due to their nonexistent operational carbon and water footprints and low operational energy footprints. 
Hydrogen Fuel Cells in Data Centers: A Clean Energy Revolution states,

>"Hydrogen fuel cells are advanced energy systems that convert hydrogen gas into electricity through a chemical reaction with oxygen. This environmentally friendly process produces only water as a byproduct, making it an exceptionally sustainable choice for powering data centers. Unlike intermittent power sources, hydrogen fuel cells provide a reliable and efficient energy supply that is crucial for data centers, ensuring clean and continuous power when needed most" (Saathoff 2024). 

The very fact that hydrogen fuel cells produce water as a byproduct means that, if such a fuel cell were installed in a data center in Chicago, the water produced by the fuel cell can either supplement water from Lake Michigan for cooling a data center or be returned to Lake Michigan (if adequate filtration systems are utilized first). 
In the former case, the fuel cell would have zero water consumption and withdrawal footprints. 
In the latter case, both of these footprints would be negative!
Like solar panels, hydrogen fuel cells are a very clean source of energy at the operational scope. 
However, examining the embodied footprints of the fuel cells reveals an entirely different story--specifically, the footprints of the methods used to produce, store and transport hydrogen gas.
“Hydrogen as an Alternative Fuel: A Comprehensive Review of Challenges and Opportunities in Production, Storage, and Transportation" states,

>"The environmental sustainability of hydrogen production is heavily influenced by the methods used to generate it. According to [Fig. 2](https://www.sciencedirect.com/science/article/pii/S0360319925000382#fig2), a significant 62% of global hydrogen production relies on natural gas without carbon capture, utilization, and storage (CCUS), while 21% comes from coal. Only a small portion is produced through electrolysis, a cleaner method that can be powered by [renewable energy sources](https://www.sciencedirect.com/topics/engineering/renewable-energy-source "Learn more about renewable energy sources from ScienceDirect's AI-generated Topic Pages") like wind or solar. This heavy dependence on fossil fuels leads to considerable carbon emissions, which challenge hydrogen's potential as a truly clean and sustainable energy carrier" (Hossain Bhuiyan and Siddique 2025).

As the article explains, hydrogen produced via electrolysis powered by renewable energy sources is called "green hydrogen". 
Ideally, all pure hydrogen would be green hydrogen, but this is not currently possible due to the energy intensive nature of hydrogen extraction, subsidies to fossil fuels, and a lack of infrastructure for extracting and storing the hydrogen (Hossain Bhuiyan and Siddique 2025).

>"The extraction process often requires significant energy inputs, leading to large expenses, especially when produced from renewable electricity using electrolysis [21]. The high cost of electrolyzers and the lack of competitive pricing relative to fossil fuels pose substantial barriers to the widespread adoption of hydrogen [4,7]. The current infrastructure for the production, transportation, and storage of hydrogen is inadequate. To attain the necessary magnitude for a net-zero economy, substantial investments are necessary to provide the essential infrastructure, including pipelines, storage facilities, and refueling stations [4]."

Green hydrogen is a promising solution for its excellent operational cleanliness. 
If the necessary infrastructure is developed and policies such as carbon taxes are enacted, hydrogen fuel cells could become a more sustainable solution than solar panels for powering Chicago's data centers. Until then, however, solar panels appear to be the most holistically efficient and environmentally conscious option, considering current trends in manufacturing procedures.


#Scope 3 Water Use#

Purchasing semiconductors from companies that strive to decrease their own water consumption is the most effective way and the only way a Chicago data center--or any data center, for the matter -- can reduce their Scope 3 water usage.

<!--Below are some quotations from the article “Semiconductor Manufacturing and Big Tech’s Water Challenge.” that quantify the use of water for semiconductor manufacturing.-->


>"But what really drives most of the industry's thirst for water is its need for ultrapure water that is used to rinse residue from silicon chips during the fabrication process" (James 2024).

>"Ultrapure water, which is thousands of times cleaner than drinking water, is treated through processes such as deionization and reverse osmosis to remove pollutants, minerals and other impurities that can damage chips. It takes roughly 1,400 to 1,600 gallons of municipal water to make 1,000 gallons of ultrapure water" (James 2024). 

>An average chip manufacturing facility today can use 10 million gallons of ultrapure water per day—as much water as is used by 33,000 US households every day" (James 2024).


These quotes emphasizes how large of an embodied footprint data centers harbor when semiconductors are purchased to place in their computers. 
Of course, no part of a data center's operations can reduce this footprint because it is all incurred offsite. 
The only way this footprint can be reduced is if the manufacturing companies from which data centers purchase the semiconductors make efforts to reduce or offset some of their water withdrawal and consumption footprints. 
Fortunately, there are companies that have. 
The article "A Spatially Explicit Assessment of Water Use by the Global Semiconductor Industry" states,

>"A large fab manufacturing facility may withdraw 3–5 million gallons per day for feedwater, although at high efficiency facilities like Intel, up to 80% of this will be returned to water bodies" (Frost and Hua 2017).

This quotation implicitly emphasizes that, of the massive amounts of water withdrawn to be converted into ultrapure water for cleaning silicon chips, not all of it is returned to its original source, creating a consumptive water footprint.

The same article explains that, as of 2017, "after conducting a water footprint of several of its major facilities, Intel estimates that 97.26% of its water footprint occurs during manufacturing" (Frost and Hua 2017).

However, it is important to note that this article was written in 2017. 
Since then, the semiconductor (fab) manufacturing company Intel has made massive strides in water footprint reduction. 

According to Intel's 2024-25 Corporate Responsibility Report,

>"By responsibly managing our water use, as guided by our Global Water
Policy, we aim to meet our business needs and those of our communities.
In 2024, we returned and restored 106% (by volume) of our fresh water
withdrawals to our communities through efficient water management,
water reuse, and projects funded by Intel that enabled water restoration
in local watersheds.
Our water strategy has three focus areas: reduce the water used in our
operations through innovative water conservation projects, reuse water
within our operations through investments in state-of-the-art water
treatment facilities, and restore water to our watersheds in collaboration
with nonprofit environmental organizations. As a part of our 2030 goals,
we aim to achieve net positive water2 by conserving 60 billion gallons
of water (cumulative from 2020) and funding projects that will restore
more fresh water than we consume to our local watersheds.
Our water conservation efforts saved approximately 10.5 billion gallons
of water in 2024. Since 2020, our water conservation efforts have saved
approximately 46.7 billion gallons of water, enough to sustain about
430,000 US homes for one year" (Intel, n.d.).

<!--The following quotation, also from the same report, describes the effectiveness of water treatement facilities invested in by Intel.-->

>"Our fresh water withdrawals totaled 11.1 billion gallons (41,942 megaliters) in 2024. Approximately 78% of the water used at our sites was sent back to municipal treatment operations, where it was treated so that it could be used for other purposes or to recharge surface or groundwater sources" (Intel, n.d.).

Intel has funded 20 watershed restoration projects in Arizona, three in California, three in New Mexico, one in Ohio, seven in Oregon, one in Texas, two in India, two in Costa Rica, one in Ireland, one in Malaysia, one in Mexico, and one in Vietnam.

<!--Here is where I will explain water efficiency measures taken by other semiconductor manufacturing companies. I am still working on aggregating this information from corporate sustainability reports.-->


#Conclusion#

To optimize Scope 1, 2, and 3 water usage while minimally compromising operational performance. energy efficiency, and carbon footprint, data centers in Chicago should use direct-to-chip cooling with Lake Michigan water as their primary cooling method, use electricity produced from solar panels as their main power source, and purchase semiconductors from companies that make efforts to reduce or offset the water used to produce semiconductors. 

In light of the sixfold conceptual framework and the principle of systems thinking, the use of direct-to-chip cooling with Lake Michigan water is the best way for Chicago data centers to reduce their Scope 1 water usage. 
It is relevant by directly addressing the main cause of Scope 1 water footprint in data centers (cooling). 
It is both effective and efficient because it uses water but returns the water to Lake Michigan, making its water consumption footprint zero while reducing the energy footprint incurred by air cooling systems. 
Its long term environmental impacts would be minimal as long as the heat exchangers and cooling coils involved in the cooling process are adequately resistant to corrosion and thus do not contaminate the water circulating through them. 
It is coherent because the return of Lake Michigan water to the source allows Lake Michigan water to remain accessible to Chicagoans and other communities that depend on it. 
It is sustainable because it involves the direct delivery of water to individual servers, ensuring that adequate cooling occurs on the server level regardless of the size of the data center. 
All of these points connect to systems thinking because the solution is simultaneously conscious of water and energy use. 

Similarly, the use of electricity produced by solar panels to power Chicago's data centers is the best way for such data centers to reduce Scope 2 water usage. 
It is relevant by directly addressing the main cause of Scope 2 water footprint in data centers (electricity generation). 
It was formerly an ineffective and inefficient solution due to the high energy and carbon footprints involved in the manufacturing of solar panels, but as these embodied footprints have drastically decreased in recent decades, it is becoming a much more effective and efficient solution.
I don't see any undesired significant long term environmental impacts as long as measures are taken to ensure the solar pane's sustained panel efficiencies.
Formerly, the manufacturing process of solar panels did not align with global climate efforts, but the positive strides being taken in this arena have steered the use of solar panels towards carbon reduction goals, making it an increasingly coherent solution. 
It is possible that, in the near future, Chicago's data centers might scale up to the point where solar electricity alone isn't enough to power them. 
For this reason, investment into and development of green hydrogen production methods are necessary to allow for the eventual transition from solar power to hydrogen fuel cells or a hybrid solar/hydrogen fuel system. 

Finally, the purchase of semiconductors from manufacturing companies that have water-saving strategies at the forefront of their operations is the best way for data centers to reduce Scope 3 water use. 
Its relevance comes from the fact that the majority of such companies' water use is form the manufacturing process (World Economic Forum 2024), as was formerly the case with the company Intel (Frost and Hua 2017).
Effectiveness and ethical coherence are established via the solutions implemented by the companies, such as water recycling methods and watershed restoration projects. 
Coherence is also established by the reporting of water efficient semiconductor manufacturing processes via corporate sustainability reports, which highlights these companies' commitment to transparency. 
Efficiency is irrelevant in this case since the efforts taken by semiconductor manufacturing companies all take place offsite and thus do not impact the performance of data centers purchasing the semiconductors, assuming the semiconductors remain of adequate quality to function properly inside a server. 
Data centers purchasing semiconductors from such companies allows the companies to continue funding water saving efforts, meaning this solution can only have positive long term environmental impacts. 
Additionally, recycling some of the water used to produce a semiconductor allows for additional water to be used to produce more semiconductors, which could allow semiconductor manufacturing facilities to upscale their production (to a degree) in response to increased data center demand. 

<!--Revise the structure of these paragraphs to remove their box-ticking tone.-->

<!--Explain the inherent limitations of not exploring data centers' carbon emissions and energy footprints in depth, despite considering these footprints to some degree when discussing water efficient solutions.-->

<!--Follow this with a list of sources a reader can explore to further educate themselves on these footprints.-->

I focused on the measures data centers can take to reduce their water footprints at the level of cooling system design, power sources, and semiconductor purchases. 
However, user queries are what ultimately drive the operation of AI models in data centers. 
Perhaps another part of the solution is for smaller businesses and individuals to make wiser use of AI, so as not to overly tax the data center servers and reduce the amount of water consumed in query processing. 
So what are "wise" and "unwise" ways for individuals to use AI?


#Preliminary bibliography (to be replaced by Markdown citation keys once I am certain of all the sources I will and won't use)#


Everman, Brad, Trevor Villwock, Dayuan Chen, Noe Soto, Oliver Zhang, and Ziliang Zong. 2023. “Evaluating the Carbon Impact of Large Language Models at the Inference Stage.” 2023 IEEE International Performance, Computing, and Communications Conference (IPCCC), November, 150–57. https://doi.org/10.1109/IPCCC59175.2023.10253886.

“Electricity Use in Homes - U.S. Energy Information Administration (EIA).” 2023. December 18. https://www.eia.gov/energyexplained/use-of-energy/electricity-use-in-homes.php.

Topp-Mugglestone, Jonas. n.d. “Data Centre Glossary (Dictionary): Key Definitions & Insights.” STL Partners. Accessed October 25, 2025. https://stlpartners.com/articles/data-centres/data-centres-glossary/.

Li, Pengfei, Jianyi Yang, Mohammad A. Islam, and Shaolei Ren. 2025. “Making AI Less ‘Thirsty.’” Commun. ACM 68 (7): 54–61. https://doi.org/10.1145/3724499.

Hiremath, Rahul B. 2024. “AI-Embedded Data Centres: Promoting Sustainability and Reducing Water Footprint.” 2024 First International Conference on Data, Computation and Communication (ICDCC), November, 40–44. https://doi.org/10.1109/ICDCC62744.2024.10961316.

Mu, Haizhi, Youqi Lu, Carter Lepre, Christina Lightfoot, Cassim Smiley, and Rheagan Crenshaw. 2025. “Artificial Intelligence and Its Carbon Footprint.” 2025 Systems and Information Engineering Design Symposium (SIEDS), May, 31–35. https://doi.org/10.1109/SIEDS65500.2025.11021149.

Vaccaro, Viviana, Lavinia Chiara Tagliabue, and Marco Aldinucci. 2025. “Sustainable Data Centers: Advancing Energy Efficiency and Resource Optimization.” 2025 33rd Euromicro International Conference on Parallel, Distributed, and Network-Based Processing (PDP), March, 486–93. https://doi.org/10.1109/PDP66500.2025.00075.

Hernandez, R. R., S. B. Easter, M. L. Murphy-Mariscal, et al. 2014. “Environmental Impacts of Utility-Scale Solar Energy.” Renewable and Sustainable Energy Reviews 29 (January): 766–79. https://doi.org/10.1016/j.rser.2013.08.041.

david. 2025. “Solar Panel Life Cycle Costs: What Illinois Property Owners Need to Know.” Illinois Renewables, February 28. https://www.illinoisrenew.org/uncategorized/solar-panel-life-cycle-costs-what-illinois-property-owners-need-to-know/.

jack. 2025. “How Solar Manufacturers Are Revolutionizing Clean Production Methods.” Mose Solar, May 3. https://www.moserbaersolar.com/uncategorized/how-solar-manufacturers-are-revolutionizing-clean-production-methods/.

Kaczmarczyk, Michał, Anna Sowiżdżał, Barbara Tomaszewska, Michał Kaczmarczyk, Anna Sowiżdżał, and Barbara Tomaszewska. 2024. “Life Cycle and Water Footprint Assessment in the Geothermal Energy Sector.” Energies 17 (23). https://doi.org/10.3390/en17236050.

King, Ben, Wilson Ricks, Nathan Pastorek, and John Larsen. 2025. “The Potential for Geothermal Energy to Meet Growing Data Center Electricity Demand.” March 11. https://rhg.com/research/geothermal-data-center-electricity-demand/.

Saathoff, Sandra. 2024. Hydrogen Fuel Cells in Data Centers: A Clean Energy Revolution - Plug Power. August 28. https://www.plugpower.com/blog/hydrogen-fuel-cells-in-data-centers-a-clean-energy-revolution/.

Hossain Bhuiyan, Md Monjur, and Zahed Siddique. 2025. “Hydrogen as an Alternative Fuel: A Comprehensive Review of Challenges and Opportunities in Production, Storage, and Transportation.” International Journal of Hydrogen Energy 102 (February): 1026–44. https://doi.org/10.1016/j.ijhydene.2025.01.033.

James, Kirsten. 2024. “Semiconductor Manufacturing and Big Tech’s Water Challenge.” World Economic Forum, July 19. https://www.weforum.org/stories/2024/07/the-water-challenge-for-semiconductor-manufacturing-and-big-tech-what-needs-to-be-done/.

Frost, Kali, and Inez Hua. 2017. “A Spatially Explicit Assessment of Water Use by the Global Semiconductor Industry.” 2017 IEEE Conference on Technologies for Sustainability (SusTech), November, 1–5. https://doi.org/10.1109/SusTech.2017.8333525.

Intel. n.d. “Intel Corporate Responsibility Report Builder.” Accessed November 8, 2025. https://www.intel.com/content/www/us/en/corporate-responsibility/csr-report-builder.html.











































