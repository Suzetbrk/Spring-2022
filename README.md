# Spring-2022

The dataset is an archive that contains power consumption measurements gathered in a house located outside Paris, France between December 2006 and November 2010 (47 months).
The dataset contains some missing values in the measurements (nearly 1,25% of the rows). All calendar time stamps are present but for some timestamps, the measurement values are missing. To fix this i imputed the missing values with the value that came right before. I believe this is an acceptable strategy because the measurements are collected every minute, and my assumption is that power consumption may vary on an monthly, hourly or daily basis and not from one minute to the next.

I am interested in seeing how power consumption changes throughout the day, and throughout the year. For the modeling part of the project I aggregated monthly data. Although it would have been interesting to look at hourly data, aggregation had the effect or reducing the size of the dataset and thus made computations much faster.

Some of the variables in the dataset are:
* Date in format dd/mm/yyyy,time in format hh:mm:ss 
* global_active_power: household global minute-averaged active power (in kilowatt) 
* global_reactive_power: household global minute-averaged reactive power (in kilowatt) 
* voltage: minute-averaged voltage (in volt) 
* global_intensity: household global minute-averaged current intensity (in ampere) 
I the following analysis focus on **global_active_power**
