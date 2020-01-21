# Running a job with R

## The answer

This should be easy for you now, but if it's not, here's the answer, just in case.

```
executable = run-r.sh
arguments = demo.r
transfer_input_files = demo.r
log = R.log.$(Cluster).$(Process)
error = R.err.$(Cluster).$(Process)
output = R.out.$(Cluster).$(Process)
queue  
```

