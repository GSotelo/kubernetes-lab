# Faster Development Cycles

Moving quickly in development isn’t just about releasing many features — it’s about making updates without impacting availability. Kubernetes supports this through tools built on key principles like:

- Immutability
- Declarative configuration
- Online self-healing systems
- Shared reusable libraries and tools

# Immutability
Containers and Kubernetes are built around the principle of immutability. Once an artifact—such as a container image—is created, it is not intended to be modified by users. Instead of applying incremental updates, a new image is built and deployed to replace the previous one. This approach offers the advantage of traceability: each change is tied to a specific image, making it easier to understand what led to a particular outcome. If something goes wrong, the system can simply roll back to a previous version. Immutable container images are a foundational concept in Kubernetes. Directly modifying a running container is considered an antipattern and should only be used as a last resort, typically in rare, time-critical production incidents where no other option is immediately viable.

