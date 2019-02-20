# Scibernetes

[Idea pitched at the [eLife Innovation Sprint 2018](), see [slide](https://docs.google.com/presentation/d/1gvyoGW-__7k41KFN4PLhZtpapHNr-4IoeMTIXMiFHDs/edit#slide=id.g37b02a27cf_47_0).]

Containers are great for capturing computational environments, the scientist’s "virtual laboratory", and provide portability and quick interactions.
They lack (intentionally for the original use case) documentation of hardware (GPU, CPU) and system (OS, Kernel) requirements as well as software licenses, but those might be relevant for scientific computing, reproducibility, and preservation.

_With Scibernetes_ we can try to demonstrate that Kubernetes can be extended to automatically schedule a container on the most suitable host/pod based on the image’s metadata (e.g. pod A having kernel 3.10 and an Nvidia GPU and pod B having kernel 4.13, exactly 8 cores and manifold software licenses, the image needing kernel 4.10 will end up on pod B while the image needing an Nvidia GPU and Kernel 4.0 will end up on pod A).

_What's needed?_ Kubernetes user/maintainer/developer, container experts, computational scientists with a very peculiar analysis environment, cloud experts.

_Scibernetes_ could be the basis for a [Binder](http://mybinder.org/) instance that spawns containers in the most suitable environment.
It might even be combined with a preservation-focussed (see also [Emsley et al.](https:/(10.2218/ijdc.v12i2.509), [Rechert et al.](https://doi.org/10.11588/heibooks.285.377)) container format, based on the OCI specification, that strips away all things that are not needed for reproducible scientific workflows (or introduces limits not affecting the majority of workflows).

_Like the idea?_ Get in touch: [@nuest](https://github.com/nuest/), [https://nordholmen.net/](https://nordholmen.net/)

------

[https://github.com/scibernetes/](https://github.com/scibernetes/)
