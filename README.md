# simulink_pcorke

Screenshot #1 (Screen Shot 2020-11-02 at 11.26.12) 
is the demonstration of first approach:
joint positions PID gains only -- proportional gains are applied only to joint angle positions, q.

Screenshot #2 (Screen Shot 2020-11-02 at 11.43.34)
is the system output for approach 1

MIMOforRRR - is the simulink file for 1st approach.

Screenshot #3 (Screen Shot 2020-11-02 at 11.47.27)
is the demonstration of second approach:
joint positions PID plus only gravity compensation (variable ArmModel) -- feed-forward error is added to joint angle position error after the PID regulator in 1st approach. Set the inertia matrix elements are ZERO.
It has both position error in scope #2 and output of the system in scope.

Screenshot #4  (Screen Shot 2020-11-02 at 11.50.18)
is the demonstration of third approach:
joint positions PID plus inverse dynamic model (variable Arm) plus joint velocity PID – feed- forward error is added to joint angle position error after the above PID regulator. Inertia elements are not zero. Joint velocity error (after its own PID) is added to the joint position error.
Scope 2 - error of position gain
Scope 1 - error of velocity gain
Scope - output of the system

!!!IN THIS CASE INERTIA AND MASSES ARE SET TO ZERO

Screenshot #5 (Screen Shot 2020-11-02 at 11.56.38)
is again third approach, but with inertia and masses set to real values.
Scope 2 - error of position gain
Scope 1 - error of velocity gain
Scope - output of the system
