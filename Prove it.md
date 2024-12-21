# Table Proof


| number | arms_down | alarm_on | northbound_present | southbound_present | north_approach  | south_approach | north_depart | south_depart | time_elapsed | safety_hazard |
|--------|-----------|----------|--------------------|--------------------|-----------------|----------------|--------------|--------------|--------------|---------------|
| 0      | 0         | 0        | 0                  | 0                  |  6              | 5              | 22           | 22           | 22           | -             |
| 1      | 0         | 0        | 0                  | 1                  |  -              | -              | -            | -            | -            |  16, 17       |
| 2      | 0         | 0        | 1                  | 0                  |  -              | -              | -            | -            | -            |  16, 17       |
| 3      | 0         | 0        | 1                  | 1                  |  -              | -              | -            | -            | -            |  16, 17, 20   |
| 4      | 0         | 1        | 0                  | 0                  |  6              | 5              | 22           | 22           | 0            | -             |
| 6      | 0         | 1        | 1                  | 0                  |  6              | 7              | 17           | 22           | 14           | -             |
| 5      | 0         | 1        | 0                  | 1                  |  7              | 5              | 22           | 17           | 13           | -             |
| 7      | 0         | 1        | 1                  | 1                  |  7              | 7              | 17           | 17           | 15           | 17, 20        |
| 8      | 1         | 0        | 0                  | 0                  |  -              | -              | -            | -            | -            | 17, 18        |
| 9      | 1         | 0        | 0                  | 1                  |  -              | -              | -            | -            | -            | 16, 18        |
| 10     | 1         | 0        | 1                  | 0                  |  -              | -              | -            | -            | -            | 16, 18        |
| 11     | 1         | 0        | 1                  | 1                  |  -              | -              | -            | -            | -            | 16, 18, 20    |
| 12     | 1         | 1        | 0                  | 0                  |  -              | -              | -            | -            | -            | 16, 17        |
| 13     | 1         | 1        | 0                  | 1                  |  15             | 13             | 22           | 4            | 16           |               |
| 14     | 1         | 1        | 1                  | 0                  |  14             | 15             | 4            | -            | 16           |               |
| 15     | 1         | 1        | 1                  | 1                  |  15             | 15             | 13           | 14           | 16           |               |

| number | invariant |
|--------|-----------|
| 16     | The alarm remains active while a train is present.      | 
| 17     | The barrier stays down until all trains depart.          | 
| 18     | Power interruptions never cause unsafe states.          |
| 19     | When power is interrupted, the alarm system stay on , or previous state       |
| 20     | If a second train enters while the sequence is active, arms and alarms should remain activated until all trains have departed.          |
| 21     | The ringing (time elapsed) should keep the alarm on for at least 10 seconds after a train departs         |
| 22     | False sensor reading |


# Specification vs. implementation
## Table's FSM



## Is your new FSM equivalent to the FSMs from the previously steps?
Yes I think that it mostly covers what our previous designs did.

<img src="docs/Prove-It-FSM.svg">