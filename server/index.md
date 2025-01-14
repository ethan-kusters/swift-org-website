---
redirect_from: "/server-apis/"
layout: page
title: Swift on Server
---

Swift is a general-purpose programming language built using a modern approach to safety, performance, and software design patterns.

The goal of the Swift project is to create the best available language for uses ranging from systems programming, to mobile and desktop apps, scaling up to cloud services.
Most importantly, Swift is designed to make writing and maintaining correct programs easier for the developer.

## Why Swift on Server?

In addition to the characteristics of Swift that make it an excellent general-purpose programming language,
it also has unique characteristics that make it specifically suitable for Server applications

### Small footprint
One of the main goals of a modern cloud platform is to maximize resource utilization by efficiently packing services into a single machine.
Cloud services built with Swift have a small memory footprint (measured in MB)--especially when compared to other popular server languages with automatic memory management.
Services built with Swift are also CPU-efficient, given the language’s focus on performance.

### Quick startup time
Swift-based applications start quickly since there are almost no warm up operations.
This makes Swift a great fit for cloud services, which are often re-scheduled onto new VMs or containers to address platform formation changes.
Using Swift also helps streamline continuous delivery pipelines, since you incur less wait time for new versions of the service fleet to come online.
Finally, quick boot times make Swift a perfect fit for serveless applications such as Cloud Functions or Lambda with negligible cold start times.

### Deterministic performance
Swift’s use of ARC (instead of tracing garbage collection) and its lack of JIT gives it an important edge in the cloud services space.
While tracing garbage collection technologies have vastly improved in the last few years, they still compete with the application for resources which triggers non-deterministic performance.
The absence of JIT means no runtime optimization or de-optimization.
It’s challenging to debug non-deterministic performance, and language-induced non-deterministic performance can both confuse and mask application-level performance issues that could otherwise be addressed.


## Swift Server Workgroup

The Swift Server work group is a steering team that promotes the use of Swift for developing and deploying server applications.
The Swift Server work group:

* Defines and prioritize efforts that address the needs of the Swift server community
* Defines and run an incubation process for these efforts to reduce duplication of effort, increase compatibility and promote best practices
* Channels feedback for Swift language features needed by the server development community to the Swift Core Team

Read more about the workgroup and server incubator it runs [here]({{site.url}}/sswg).

## Development guides

The following guides have been developed by the Swift Server work group and the Swift on Server community.
They are designed to help teams and individuals running Swift Server applications on Linux and to provide orientation for those who want to start with such development.
They focus on how to compile, test, deploy and debug such application and provides tips in those areas.

- [Setup and code editing](https://github.com/swift-server/guides/blob/main/docs/setup-and-ide-alternatives.md)
- [Building](https://github.com/swift-server/guides/blob/main/docs/building.md)
- [Testing](https://github.com/swift-server/guides/blob/main/docs/testing.md)
- [Debugging Memory leaks](https://github.com/swift-server/guides/blob/main/docs/memory-leaks-and-usage.md)
- [Performance troubleshooting and analysis](https://github.com/swift-server/guides/blob/main/docs/performance.md)
- [Debugging multithreading issues and memory checks](https://github.com/swift-server/guides/blob/main/docs/llvm-sanitizers.md)
- [Deployment](https://github.com/swift-server/guides/blob/main/docs/deployment.md)

_These guides are community effort, and all are invited to share their tips and know-how by submitting pull requests to the [source repository](https://github.com/swift-server/guides)_.
