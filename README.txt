== This is the Readme file for folder FSM_files ==

/abstracted 
contains 10 automata models. Four of them (temp1, temp2, temp5, subsys3) are obtained from abstraction, where tempi is abstracted from Gi_t and other related variable automata. The remaining 6 automata are variable automata that were excluded in the abstraction process. They should be included in the full parallel composition.

To obtain the “full abstracted model”, we compose all of the 10 automata + faultFSM.fsm (we will explain faultFSM.fsm later)

=============================================

/abstracted_no-typo
contains 10 automata models. These are the “no-typo” version of abstracted models. To obtain the “full abstracted model”, we compose all of the 10 automata + faultFSM_no-typo.fsm 

=============================================

/faultSpec
contains 2 specification automata that are used to enforce the order of events we need for modeling faults. Note that the typo in the TRW source codes is modeled in the faultSpec automata. Specifically, faultFSM.fsm models the original source codes that contains the typo, and faultFSM_no-typo.fsm models the source codes after we manually correct the typo.
  
=============================================

/raw
contains 29 automata. 4 of them (Gi_t.fsm) are basic automata and 24 of them are variable automata. Note that we remove the trunk in the models. No automata here should be relevant to the trunk. 

=============================================
/testcase

4 test cases that are used to test the blocking search tool
