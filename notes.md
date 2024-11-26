# sketch of procedure for students
* get yourself to about 2000 atoms (can gradually drag up as dynamics runs, the "freeze" button might be helpful to give yourself space)
* use "faster" button to get to a temperature of about 0.5
* for "mouse/touch" choose "Select" and pick an atom
* unhide "Data" section at the bottom, choose "Selected atom" for data type, and set "Auto interval" to 10 (TBD)
* let dynamics run to collect data for awhile
* paste into a text box to collect data for a single atom at a few different temperatures
* ...

# notes to self
## to get local copy running (eventually will need to clone into ChemCompute using image 1.9):
* `juliaup add 1.5.3`, `julia +1.5.3`
* add IJulia, Conda to base environment
* run
  ```julia
  using Conda
  Conda.pip_interop(true)
  Conda.pip("install", "webio_jupyter_extension")
  ```
* `using IJulia; notebook(dir="local/path/to/repo/")`