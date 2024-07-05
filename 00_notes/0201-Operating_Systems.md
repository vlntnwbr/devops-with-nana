Memory Swapping -> Means clearing the memory of process data to make space for
other process data.

Memory data does not persist, therefore storage is needed. An OS saves data from
memory in a structured (hierarchical) way in order to persist it.

Another task is interfacing with hardware, networking and security. To manage
this shit Operating Systems use Users that have permissions.


Kernel loads first. The heart of every OS, manages the internal and external
Hardware (they use drivers for that).

On top of the Kernel there is the Application Layers, e.g. different Linux
Distros have differing Application Layers but they're based on the same Kernel.
The Linux Kernel is also used by Android.

## POSIX -Portable Operating System Interface

Is a standard that ensures compatibility of most UNIX-like operating systems.
Both MacOS (formerly OS X) are POSIX-compliant.