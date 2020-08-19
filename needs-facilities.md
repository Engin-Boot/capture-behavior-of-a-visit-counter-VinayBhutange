# Visit-counter for a Facilities Manager

## Scenario: Report visitor trends during a week of operation

  Given : Count data of visitors of previous week and hospital issues the id card to every visitors.
  
  When : Starting day of new week.
  
  Then : Publish the data of previous week.

## Scenario: Alert when seating capacity is full

  Given : The data of visitors and an alert system is available.
  
  When : The number of visitors crosses the maximum limit of seats.
  
  Then : Alert the respective department for the action.
