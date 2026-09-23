# uDALES submission pattern

Move the submission files into the `uDALES` folder root and then submit them like this:

```bash
JOBID=$(qsub run_sim.pbs)
qsub -W depend=afterok:$JOBID merge_output.pbs
```
