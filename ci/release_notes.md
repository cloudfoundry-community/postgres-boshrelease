## Improvements

- Postgres deployed as HA will now shutdown in cases of split-brain.
- Added an errand to help recover Postgres VMs after a failure mode.

If the two nodes notice both are master (which can occur in certain
cases, see README.md for more information), we have opted to have
both VMs shut down their Postgres processes in the interest of
data integrity. To assist in this process, we have added an errand
to start the processes again. Please see README.md for more
information on this process.