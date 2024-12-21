## Eddie's FSM 
- Counter Examples:
    - If NorthBoundApproach occurs & we are in any state except "Idle" and SouthBoundApproach then occurs, we would raise the barrier when NorthBoundDepart happens. This would create a situation where the barrier is in the raised position but a train is still in the critical section.
    - Similar to the first counterexample, if more than NorthBoundAproach or SouthBoundApproach occurs before reaching the idle state, again we would reach a state where the barrier is up, but trains are present. 

## Noah's FSM
Noah Prelab FSM

<img src="docs/Noah Prelab Fsm.jpg">


Noah Fixed FSM

<img src="docs/Noah Fixed Fsm.svg">

Eddie Fixed FSM

<img src="docs/eddie fsm fixed.jpeg">
