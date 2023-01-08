# BCG_Project

## PowerCo Case Task Description

### The task

We have scheduled a meeting in one week's time with the head of the SME division in which you will present our findings of the churn issue and your recommendations on how to address it.

You are in charge of building the model and of suggesting which commercial actions should be taken as a result of the model's outcome.

### Modelling and presentation requirements

* The first stage is to establish the viability of such a model. For training your model you are provided with a dataset which includes features of SME customers in January 2016 as well as the information about whether or not they have churned by March 2016. In addition to that you have received the prices from 2015 for these customers. Of particular interest for the client is how you frame the problem for training.

* Given that this is the first time the client is resorting to predictive modelling, it is beneficial to leverage descriptive statistics and visualization for extracting interesting insights from the provided data before diving into the model.

* Finally, the client would like to have a view on whether the 20% discount offer to customers predicted is a good measure. Given that it is a steep discount – bringing their price lower than all competitors – we can assume for now that everyone who is offered the discount will accept it. According to regulations, PowerCo cannot raise the price of someone within a year if they accept the discount. Therefore, offering it excessively is going to hit revenues hard.





## Data Description

client_data.csv 

[data source](https://cdn.theforage.com/vinternships/companyassets/SKZxezskWgmFjRvj9/BqF6gmrmLunCkdqKM/1639044685365/client_data.csv)

  - id = client company identifier
  -	activity_new = category of the company’s activity
  -	channel_sales = code of the sales channel
  -	cons_12m = electricity consumption of the past 12 months
  -	cons_gas_12m = gas consumption of the past 12 months
  -	cons_last_month = electricity consumption of the last month
  -	date_activ = date of activation of the contract
  -	date_end = registered date of the end of the contract
  -	date_modif_prod = date of the last modification of the product
  -	date_renewal = date of the next contract renewal
  -	forecast_cons_12m = forecasted electricity consumption for next 12 months
  -	forecast_cons_year = forecasted electricity consumption for the next calendar year
  -	forecast_discount_energy = forecasted value of current discount
  -	forecast_meter_rent_12m = forecasted bill of meter rental for the next 2 months
  -	forecast_price_energy_off_peak = forecasted energy price for 1st period (off peak)
  -	forecast_price_energy_peak = forecasted energy price for 2nd period (peak)
  -	forecast_price_pow_off_peak = forecasted power price for 1st period (off peak)
  -	has_gas = indicated if client is also a gas client
  -	imp_cons = current paid consumption
  -	margin_gross_pow_ele = gross margin on power subscription
  -	margin_net_pow_ele = net margin on power subscription
  -	nb_prod_act = number of active products and services
  -	net_margin = total net margin
  -	num_years_antig = antiquity of the client (in number of years)
  -	origin_up = code of the electricity campaign the customer first subscribed to
  -	pow_max = subscribed power
  -	churn = has the client churned over the next 3 months

price_data.csv

[data source](https://cdn.theforage.com/vinternships/companyassets/SKZxezskWgmFjRvj9/BqF6gmrmLunCkdqKM/1639044717433/price_data.csv)

  -	id = client company identifier
  -	price_date = reference date
  -	price_off_peak_var = price of energy for the 1st period (off peak)
  -	price_peak_var = price of energy for the 2nd period (peak)
  -	price_mid_peak_var = price of energy for the 3rd period (mid peak)
  -	price_off_peak_fix = price of power for the 1st period (off peak)
  -	price_peak_fix = price of power for the 2nd period (peak)
  -	price_mid_peak_fix = price of power for the 3rd period (mid peak)

Note: some fields are hashed text strings. This preserves the privacy of the original data but the commercial meaning is retained and so they may have predictive power
