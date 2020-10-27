# CitiBikeDataViz
<h2> Exploring data from Citi Bike using Tableau </h2>

Citi Bike is the nation's largest bike share program, with 12,000 bikes and 750 stations across Manhattan, Brooklyn, Queens and Jersey City.  It can be used for quick trips with convenience in mind, and it’s also a fun and affordable way to get around town.

**Note:** Since the Tableau workbook file is too large for Github to process, below I have uploaded pictures of my visualizations.

**The following dataset contains bike sharing transactions for July, August, and September 2019 located in Jersey City, NJ with the following attributes:**

tripduration  (seconds)

starttime:  (Excel date & time format)

stoptime:  (Excel date & time format)

start_station_id  (integer)

start_station_name  (alphanumeric)

start_station_latitude  (latitude)

start_station_longitude  (longitude)

end_station_id  (integer)

end_station_name  (alphanumeric)

end_station_latitude  (latitude)

end_station_longitude  longitude)

bike_id  (integer)

usertype  (Customer = time based rental, Subscriber = annual member)

birthyear (integer, yyyy)

gender (integer, Zero=unknown, 1=male, 2=female)

### Feature Engineering

**converting seconds to hours**
In order to have converted tripduration from seconds to hours, I divided tripduration by 3600 and then multiplied by 60 which I then made into a new variable labeled TriptoHours

**converting Gender category into a string**

This was done so that it could be easily visualized by an audience, rather than having them try to figure out what 1 or 2 signifies. I converted the binary integer variable by using the following conditional statement:

`IF [Gender]=1
THEN 'Male'
ELSEIF [Gender]=2
THEN 'Female'
END`

### Now finally some visualizations :rocket:

![AvgTripPerStartingStation](https://user-images.githubusercontent.com/72951594/97278147-c4c8c480-180f-11eb-97fe-f31dd1efca62.png)
 
 ![StartEndAvgHour](https://user-images.githubusercontent.com/72951594/97278266-f0e44580-180f-11eb-9507-d93fd322929e.png)

![Stackedbar](https://user-images.githubusercontent.com/72951594/97278365-13765e80-1810-11eb-8333-bade19acafe0.png)

![TopTen](https://user-images.githubusercontent.com/72951594/97278407-238e3e00-1810-11eb-9ef2-5b086185fa89.png)

![AvgTripbyGender User](https://user-images.githubusercontent.com/72951594/97278459-34d74a80-1810-11eb-9bab-b9d7f010c161.png)
