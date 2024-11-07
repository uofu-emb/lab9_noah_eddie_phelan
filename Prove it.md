# Table Proof


| number | arms_down | alarm_on | northbound_present | southbound_present | north_approach  | south_approach | north_depart | south_depart | ringing | safety_hazard |
|--------|-----------|----------|--------------------|--------------------|-----------------|----------------|--------------|--------------|---------|---------------|
| 0      | 0         | 0        | 0                  | 0                  |  6              | 5              | -            | -            | 21       | -             |
| 1      | 0         | 0        | 0                  | 1                  |  -              | -              | -            | -            | -       |  16, 17    |
| 2      | 0         | 0        | 1                  | 0                  |  -              | -              | -            | -            | -       |  16, 17    |
| 3      | 0         | 0        | 1                  | 1                  |  20             | 20             | -            | -            | 21       |  16, 17, 20   |
| 4      | 0         | 1        | 0                  | 0                  |  6              | 5              | 17, 0        | 17, 0        | 21       | 16           |
| 5      | 0         | 1        | 0                  | 1                  |  7              | 8              | -            | 4            | 21       | 17        |
| 6      | 0         | 1        | 1                  | 0                  |  8              | 7              | 4            | -            | 1       | 17        |
| 7      | 0         | 1        | 1                  | 1                  |  6              | 5              | 21           | 21           | 5       | 17, 20        |
| 8      | 1         | 0        | 0                  | 0                  |  -              | -              | -            | -            | 21       | 17, 18            |
| 9      | 1         | 0        | 0                  | 1                  |  -              | -              | -            | -            | -       | 16, 18        |
| 10     | 1         | 0        | 1                  | 0                  |  -              | -              | -            | -            | -       | 16, 18        |
| 11     | 1         | 0        | 1                  | 1                  |  -              | -              | -            | -            | -       | 16, 18, 20        |
| 12     | 1         | 1        | 0                  | 0                  |  -              | -              | -            | -            | -       | 16, 17       |
| 13     | 1         | 1        | 0                  | 1                  |  -              | -              | -            | 4            | -       | 17            |
| 14     | 1         | 1        | 1                  | 0                  |  -              | -              | 4            | -            | 1       | 17            |
| 15     | 1         | 1        | 1                  | 1                  |  6              | 5              | 14           | 13           | 1       | 17, 20            |

| number | invariant |
|--------|-----------|
| 16     | The alarm remains active while a train is present.      | 
| 17     | The barrier stays down until all trains depart.          | 
| 18     | Power interruptions never cause unsafe states.          |
| 19     | When power is interrupted, the alarm system stay on , or previous state       |
| 20     | If a second train enters while the sequence is active, arms and alarms should remain activated until all trains have departed.          |
| 21     | The ringing (time elapsed) should keep the alarm on for at least 10 seconds after a train departs         |


<img src="docs/FSM From Table - Sheet1 (1).svg">
# Specification vs. implementation
## Table's FSM



## Is your new FSM equivalent to the FSMs from the previously steps?
