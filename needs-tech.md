# Visit-counter technical needs

Scenario: Recover across restarts of the server that runs the visit-counter

  Given the server is down, there is a backup server, backup server is active
  When the server restarts, server sends request to backup server to get visitor count data
  Then visitor count data is retrieved

Scenario: Reconcile counts if the sensor is offline for a while

  Given
  When
  Then
