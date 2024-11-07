# Table Proof


| number | arms_down | alarm_on | northbound_present | southbound_present | north_approach  | south_approach | north_depart | south_depart | ringing | safety_hazard |
|--------|-----------|----------|--------------------|--------------------|-----------------|----------------|--------------|--------------|---------|---------------|
| 0      | 0         | 0        | 0                  | 0                  |  0              | 0              | 0            | 0            | 0       | no            |
| 1      | 0         | 0        | 0                  | 1                  |  0              | 1              | 0            | 0            | 0       | yes 16, 17    |
| 2      | 0         | 0        | 1                  | 0                  |  1              | 0              | 0            | 0            | 0       | yes 16, 17    |
| 3      | 0         | 0        | 1                  | 1                  |  1              | 1              | 0            | 0            | 0       | yes 16, 17    |
| 4      | 0         | 1        | 0                  | 0                  |  0              | 0              | 0            | 0            | 1       | no            |
| 5      | 0         | 1        | 0                  | 1                  |  0              | 1              | 0            | 0            | 1       | yes 17        |
| 6      | 0         | 1        | 1                  | 0                  |  1              | 0              | 0            | 0            | 1       | yes 17        |
| 7      | 0         | 1        | 1                  | 1                  |  1              | 1              | 0            | 0            | 1       | yes 17        |
| 8      | 1         | 0        | 0                  | 0                  |  0              | 0              | 0            | 0            | 0       | no            |
| 9      | 1         | 0        | 0                  | 1                  |  0              | 1              | 0            | 0            | 0       | yes 16        |
| 10     | 1         | 0        | 1                  | 0                  |  1              | 0              | 0            | 0            | 0       | yes 16        |
| 11     | 1         | 0        | 1                  | 1                  |  1              | 1              | 0            | 0            | 0       | yes 16        |
| 12     | 1         | 1        | 0                  | 0                  |  0              | 0              | 0            | 0            | 1       | no            |
| 13     | 1         | 1        | 0                  | 1                  |  0              | 0              | 0            | 1            | 1       | no            |
| 14     | 1         | 1        | 1                  | 0                  |  0              | 0              | 1            | 0            | 1       | no            |
| 15     | 1         | 1        | 1                  | 1                  |  0              | 0              | 1            | 1            | 1       | no            |

| number | invariant |
|--------|-----------|
| 16     | The alarm remains active while a train is present.      | 
| 17     | The barrier stays down until all trains depart.          | 
| 18     | Power interruptions never cause unsafe states.          |
| 19     | When power is interrupted, the alarm system stay on , or previous state       |
| 20     |           |

<img src="docs/FSM From Table - Sheet1 (1).svg">
# Specification vs. implementation
## Table's FSM



## Is your new FSM equivalent to the FSMs from the previously steps?
