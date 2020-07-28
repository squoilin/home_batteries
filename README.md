# Evaluating the value of battery storage to balance rooftop PV in Belgium: A simple open-sourced calculation

The recent dislosure of the Tesla Powerwall home battery has entailed high expectations in the energy field. Many observers predict an uptake of such PV/Battery units, which could ultimately disconnect from the grid and lead to totally autonomous home or minigrid systems. The goal of this notebook is to evaluate the profitability and potential of the 7 kWh Tesla battery in the Belgian system under different hypotheses.

For the sake of openness, the selected format is the open-source Ipython Notebook format, which allows to easily follow and check all calculations and hypotheses. The input data is public data and is also made available through csv files. The original ipynb file can be downloaded here and allows further reuse/modification/adaptation of the notebook.

All comments and suggestion are very welcome.

Sylvain Quoilin

Researcher at the European Commission (JRC) and at the University of Liege.

E-mail: sylvain.quoilin@ec.europa.eu - Twitter: @squoilin

NB: The views expressed are purely those of the author and may not in any circumstances be regarded as stating an official position of the European Commission.

May 2015


Key findings
------------
For a standard household with a 3.7 kWp PV system, using a Tesla-type battery of 7 kWh results in levelized stored energy cost of 195 EUR/MWh. Adding a levelized cost of 110 EUR/MWh for the rooftop PV, the total cost is about 305 EUR/MWh. As a comparison, the average retail price in Belgium is about 220 EUR/MWh

In these conditions, the average depth of charge/discharge is 53%, corresponding to 1940 full equivalent discharge cycle of the battery over its lifetime. The self consumption rate is 68%. Higher self consumption rates would entail higher levelized cost of stored energy.

The "net metering" pricing scheme is not suitable for the addition of a battery into a grid-connected PV system. This scheme is indeed blind to the timing of PV production, and installing a battery adds an additional cost and additional round-trip losses. Without battery, the average houshold expense for one MWh is 117 EUR/MWh. With battery, this expenses increases up to 193 EUR/MWh

The 7 kWh battery does not allow to go off-grid, even with higher installed capacity. With a value of lost load of 1000 EUR/MWh and an oversized PV system of 6 kWp, the optimum sizing still results in insufficient electricity supply during 20% of the time. Other flexibility mechanisms (eg demand side management) or power generation units (e.g. wind) should be added to the system.

Battery systems require a modification of the legislative framework to become competitive: self consumption must be incentivized, e.g. by imposing a low (wholesale) price on the electricity sold to the grid and high (retail) price on the electricity bought to the grid. In this case net meters should be replaced by bi-directional meters. Nevertheless, with the current retail and wholesale prices, installing a battery still increases the average kWh cost by about 10 EUR/MWh.

In the incentivized self-consumption scheme, battery becomes competitive if one of the following conditions is satisfied: (1) its prices drops below 2217 EUR (2500 USD) (2) the retail price is higher than 252 EUR/MWh (3) the selling price is lower than 20 EUR/MWh

In conclusion, there does not seem to be a business case (yet) for the Tesla battery in the current Belgian context, especially under the net-metering framework. To make it profitable, incentives should be provided for self-consumption, such as high difference between the electricity bought and sold from and to the grid. From a system point of view, such incentives should be put in balance with alternative means to smooth out the variations of PV power in a centralized way.

![Main results](SCR2.png?raw=true "Main results")

