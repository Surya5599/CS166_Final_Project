# CS166_Final_Project

### Extra features
* View all data from DB within GUI
  * Allows for quick debugging or data lookup
* Cruise information is displayed when choosing a cruise to book
  * Allows for user to assess whether the right cruise is selected
* Ability to select captain (by name) and ship when adding a cruise
  * Allows for the population of the CruiseInfo table, making the cruise available for use by other functions
* Pop-up to create customer if customer does not exist on file when booking a cruise
    * Allows for the easy creation of new customers when booking 
* Error specific pop-ups 
    * In order to make the GUI more user-friendly
* Show next available cruise if no cruise found on date
   * Allows a user to know a valid date for a cruise if they enter a date before the departure date of a cruise  
    
---

### Assumptions
* Cruise.num_sold is equal to the amount of seats that we consider "unavailable"
* Available Seats is only relevant for cruises that have not yet departed. Otherwise we assume there are no available seats
* When adding a ship a user can add new info for Make and Model that is not within the database, and allows for numeric input
* When adding a cruise, user can add new ports information can be added and it can be numeric
---

### Modification to Schema
* DATE type replaced with TIMESTAMP for arrival and departure fields
    * Allows for more accurate time keeping where relevant. Can be ignored by user if not needed
