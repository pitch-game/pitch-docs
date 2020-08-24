# Competitions

This microservice will be responsible for calling the Match API to simulate games at a specific time related to the appropriate competition. Users can view scheduled upcoming matches for all competitions and lock in their squad before match day.

It's possible that no scheduler to trigger the call to the Match API to simulate the game is needed. At the time of the final user locking in their squad we can simulate the match with a kick off time in the future.