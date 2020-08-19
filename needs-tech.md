# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given : visit counter is connected to the central server and all the data is synced.
  When : System fails
  Then : After restart the server should be synced with all data.

Scenario: Reconcile counts if the sensor is offline for a while

  Given : Server works fine and the visit counter stores count.
  When : Sensor is offline and a visitor visits.
  Then : System changes the value of counter from an offline log.
