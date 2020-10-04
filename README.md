# INTRO

![image](https://github.com/wslu42/qShooter/blob/main/logo.png)

 **Save us from the limbo loop with quantum circuits!**

The entire disaster began when human realized how to manipulate wormhole with advanced quantum computers. A newly discovered macro-molecule leaked from the wormhole, “loopeon”, which mostly consists of two quantum anti-matter cores covered with superdense shell and connected with a loop-like bridge, can annihilate with anything with a direct contact. The source of this molecule remains unknown at this point, while so far researchers summarized below properties:

1. Our entire planet can be annihilated with merely 8 loopeons.
2. After annihilation the energy will be partially released as gamma radiation, while the rest of the energy was transferred to the other end of the wormhole. The detail of the other end is still a mystery to us, but has been referred as "the eternal limbo loop".
3. According to cosmologists, during the process when the inner core passes through the quantum wormhole, the two-core loop structure was formed and the cores are entangled.
4. The loopeon can only be destroyed when all entangled cores are annihilated simultaneously.
5. The threat of a loopeon can be neutralized if the softer inner cores were simultaniously in-contact with dense materials such as lead or Osmium. In that scenario the annihilation of inner cores will disentangle the entire loopeon and release all of the energy through gamma radiation.

As a quick response to stop this apocalypse we developed the Osmium Quantum Projector (OQP). By successfully compose a quantum circuit we are able to send out the Osmium bullets with the help to quantum superposition and/or entanglement, which annihilate the cores simultaneously and save the entire planet from further annihilation.

To prevent us from getting stuck in the loop, we need everyone's help to test out our prototype OQP. Join us to use quantum to disentangle the loop!

![image](https://github.com/wslu42/qShooter/blob/main/sc.png)


# BEHIND THE SCENE

In this work I implemented randomness, superposition and entanglement through QASM backend. The real qubit devices can be loaded but I haven't really tried since in this game device-specific parameters won't make any differences. The user control is just a three-qubit circuit composer with circuit depth = 3, and by using X, H, and CX gates we asked user to come up with states match to the falling blocks (loopeon). The measurement part of in this code is designed such that counts won't be too high that user can basically shoot down anything with H gates.

1. Has only 16 shots each time when user load the circuit with space bar.
2. For states with counts <4, set the count of that state to 0.
