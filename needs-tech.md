# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given : There is central server connected to the visit counter.
  
  When : System fails
  
  Then : System changes the value of counter in the server .

Scenario: Reconcile counts if the sensor is offline for a while

  Given : Server works fine and the visit counter stores count.
  
  When : Sensor is offline and a visitor visits.
  
  Then : System changes the value of counter from an offline log.
