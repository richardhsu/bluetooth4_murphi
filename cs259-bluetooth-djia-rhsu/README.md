Bluetooth 4.0 Murphi Modeling
=============================

Murphi Model Checking of Bluetooth 4.0 Secure Simple Pairing

Running
=======

1. Run `make` in the directory after modifying any flags necessary.
2. To run the analysis run `./bt -ndl -tv -nosym`
3. You may need the optional `-m <size_in_mb>` flag to increase memory space.
   * Example: `./bt -ndl -tv -m 5000 -nosym` to allocate 5GB of memory.

Switching Between Association Models
------------------------------------

* Change the `PHASETWO` flag on line 126 to switch between Just Works (1)
  and Numeric Comparison (2) association models.


Switching Between Initial Connection Mode
-----------------------------------------

* Change `ASSUMEVALIDRESPONDER` flag on line 127 to switch between allowing
  the initiator to connect only to honest responders (TRUE) or
  any AgentId (FALSE). 


