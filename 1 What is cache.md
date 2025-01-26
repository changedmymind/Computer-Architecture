Cache is a storage layer located inside a cpu. It's high speed and temporarily stores frecuently accessed data by the cpu.
There are different types of caches and each serve a different purpose:
- L1 cache: is located inside a cpu core, is the fastest type of cache
- L2 cache: slower than L1 and can be located inside or outside the cpu core
- L3 cache: even slower than L2, but it's shared by multiple cores in the cpu

Cache was design to make the cpu not depend on the slower speeds of RAM, as this memory runs comparatively slower than the cpu itself. 

You can see it in what is called 'die map'


Also it's possible to get details of the design of the cores themselves, called 'core micro-architecture', and it looks like this:
![[Pasted image 20250126031805.png]]

A Pentium 4 looks like this
![[Pasted image 20250126031905.png]]
