# VHDL Counter Overflow Bug

This repository demonstrates a common error in VHDL code: incorrect handling of counter overflow.  The `buggy_counter.vhd` file contains a counter that has a potential overflow issue.  The `fixed_counter.vhd` file provides a corrected version.  The bug is subtle and might not be immediately apparent during simulation, especially with shorter simulation runs. 

**Bug:** The original counter does not properly handle the case when the count reaches its maximum value (15). Instead of resetting to 0, it continues counting, leading to unpredictable behavior.

**Solution:** The solution file addresses this by explicitly resetting the counter to 0 when it reaches its maximum value. This ensures correct behavior and prevents unexpected outcomes.