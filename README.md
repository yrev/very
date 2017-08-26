# yrev

**yrev** (pronounced like *irrev*, as in *irreversible*) is a project to create
a complete operating system and software distribution, where each program or
library is a stripped-down toy version of the "real thing", and thus can be
easily understood by reading the entire source code or even typing in the
entire source code [step-by-step](http://viewsourcecode.org/snaptoken).

## How?

Source code will be kept small by ignoring three significant sources of bloat
and unnecessary complexity: optimization, portability, and interoperability.

### Optimization

This includes optimizing for CPU usage, memory usage, disk usage, network
usage, and any other resources.

Obviously some optimization is good, but code can get very messy, hacky, and/or
complex when you start trying to squeeze every last drop of optimization out of
it. Only include optimizations that cost a small amount of complexity for a
very large gain in speed (or whatever is being optimized). Try to optimize for
education.

### Portability

We will target one machine architecture, probably x86-64. People should be able
to run it directly on actual hardware, it's more satisfying.

Making breaking changes is fine and we won't worry about backward compatibility
either.

### Interoperability

We will invent our own file formats, languages, and protocols for everything.
Of course, they'll all be based on the "real thing". But we don't have to make
them interoperable with the "real thing", except for maybe hardware drivers and
TCP/IP.

