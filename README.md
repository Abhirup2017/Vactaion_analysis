# Vactaion_analysis

"""
Exercise - Data Analysis for Vacation Planning
You're planning a vacation, and you need to decide which city you want to visit. You have shortlisted four cities and identified the return flight cost, daily hotel cost, and weekly car rental cost. While renting a car, you need to pay for entire weeks, even if you return the car sooner.

City	Return Flight ($)	Hotel per day ($)	Weekly Car Rental ($)
Paris	200	20	200
London	250	30	120
Dubai	370	15	80
Mumbai	450	10	70
Answer the following questions using the data above:

If you're planning a 1-week long trip, which city should you visit to spend the least amount of money?
How does the answer to the previous question change if you change the trip's duration to four days, ten days or two weeks?
If your total budget for the trip is $1000, which city should you visit to maximize the duration of your trip? Which city should you visit if you want to minimize the duration?
How does the answer to the previous question change if your budget is $600, $2000, or $1500?
Hint: To answer these questions, it will help to define a function cost_of_trip with relevant inputs like flight cost, hotel rate, car rental rate, and duration of the trip. You may find the math.ceil function useful for calculating the total cost of car rental.

"""

def cost_of_trip(return_flight_cost,hotel_rate,car_rental, duration):
    
    total_amount = return_flight_cost+hotel_rate*duration+car_rental
    return total_amount

Paris = cost_of_trip(return_flight_cost=200, hotel_rate=20, car_rental=200, duration=4)

London = cost_of_trip(return_flight_cost=250, hotel_rate=30, car_rental=120, duration=4)

Dubai = cost_of_trip(return_flight_cost=370, hotel_rate=15, car_rental=80, duration=4)
