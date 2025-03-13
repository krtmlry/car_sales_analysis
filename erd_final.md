

dim_dealers
---
dealar_id int
dealer varchar
city varchar
country varchar

dim_models
---
model_id int
model varchar
brand_id int
segment_id int
engine_size_l float
fuel_type varchar
price_usd numeric
profit_usd numeric


fact_car_sales
---
sale_id pk int
date datetime
dealer_id int FK >- dim_dealers.dealar_id
model_id int FK >- dim_models.model_id
quantity int
unit_price numeric
unit_profit numeric
total_price numeric
total_profit numeric


