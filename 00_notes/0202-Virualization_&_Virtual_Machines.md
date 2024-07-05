Hypervisor is a technology that allows creation of Virtual Computers by asking the underlying Operating System to allocate physical hardware to the virtual one.

Virtualbox is a popular Hypervisor.

A Virtual Machine does not know it is virtual, it considers itself to be a
physical computer. This is good, because it doesn't endanger the real Computer.

These hypervisors are called Type 2.

## Type 1 (Bare-Metal) Hypervisor

Instead of installing the hypervisor as an OS-Application they are installed
directly on the hardware. Aside from that they function the same way, allocating
physical hardware to virtual computers that consider themselves to be "real".

VMware ESXi and MS Hyper-V are examples for that.

Type 1 Hypervisors are generally used on servers, not personal computers.

This is a big deal because it abstracts hardware from operating systems. That
makes it way more easier to maintain because operating systems are writable to
files, with all the benefits that come along with it (portability, backup, etc.).

Makes it also easier to snapshot Application Layer. 
