# Preliminary Final Year Project Proposal

**Project Title:** Design and Implementation of a Lightweight Daemonless Workload Execution Engine for Resource-Constrained Linux Systems Using Rust

**Project Domain:** DevOps, Cloud Infrastructure and Systems Engineering

**Project Duration:** November 2026 – March 2027 (Tentative)

## 1. Introduction

Modern software development and cloud computing environments rely extensively on workload execution, containerization, resource management and infrastructure automation. Technologies such as Docker, Podman and Kubernetes provide comprehensive solutions for managing applications and their execution environments.

However, certain workloads, particularly short-lived automated tasks, testing processes and scripts running on resource-constrained Linux servers, may not require the complete functionality of general-purpose container management platforms.

This project proposes the development of a lightweight, modular workload execution engine using Rust and native Linux operating system mechanisms.

## 2. Problem Statement

Executing applications directly on shared Linux infrastructure can result in resource contention, uncontrolled process execution and unintended access to host resources.

Although existing containerization and sandboxing tools provide mechanisms to address these challenges, there remains practical value in investigating the trade-offs associated with a specialized execution engine designed for temporary workloads and resource-constrained environments.

The proposed project will explore how workload isolation, resource enforcement and reliable process lifecycle management can be achieved through a minimal, daemonless architecture.

## 3. Project Aim

To design, develop and experimentally evaluate a lightweight workload execution engine that uses Linux operating system mechanisms to provide controlled execution, resource management and process isolation.

## 4. Project Objectives

- Develop a modular workload execution engine using the Rust programming language.
- Implement process creation, supervision and termination mechanisms.
- Provide workload isolation using supported Linux namespace mechanisms.
- Enforce CPU, memory and process limits using cgroups v2.
- Implement configurable execution policies, timeouts and resource cleanup.
- Provide a command-line interface for managing workload execution.
- Collect execution statistics and structured logs.
- Evaluate the system through comparative performance and functional experiments.
- Establish an extensible architecture for potential future integration with distributed workload management systems.

## 5. Proposed Methodology

The project will follow an iterative, prototype-driven software development methodology.

Initially, fundamental Linux process management and Rust system programming concepts will be studied and implemented through a process execution prototype.

Subsequent development phases will introduce workload isolation, resource management, execution policies, lifecycle management and testing.

The system will be evaluated using reproducible workloads and comparable configurations of established execution tools where applicable.

Experimental metrics will include startup latency, resource consumption, execution overhead, resource-limit enforcement, timeout behavior and cleanup reliability.

## 6. Proposed System Architecture

The system will consist of the following major components:

- Command-line interface and configuration parser.
- Workload execution and lifecycle management engine.
- Linux namespace-based isolation module.
- Cgroup-based resource management module.
- Process supervision and execution policy module.
- Resource cleanup and logging module.
- Performance evaluation and automated testing environment.

A web-based management dashboard, HTTP API and database may be incorporated if required by the academic project guidelines.

## 7. Tools and Technologies

**Programming Language:** Rust

**Target Operating System:** Linux

**Operating System Mechanisms:** Linux namespaces, cgroups v2, process management and privilege restrictions.

**Development Environment:** Windows Subsystem for Linux and Linux virtual machines.

**Cloud Testing Environment:** Microsoft Azure Linux servers.

**Version Control and CI/CD:** Git, GitHub and GitHub Actions.

**Optional Management Interface:** Next.js, Rust-based HTTP API and SQLite.

## 8. Expected Outcomes

The expected outcome is a functional prototype capable of executing predefined workloads within controlled Linux environments, enforcing configurable resource limits and providing execution statistics.

The project will also produce technical documentation, automated tests and a comparative evaluation of the prototype's performance and limitations.

The proposed system is intended as an experimental infrastructure engineering tool rather than a production-ready replacement for Docker, Podman or Kubernetes.

## 9. Tentative Development Schedule

| Period | Expected Deliverable |
|---|---|
| November 2026 | Project approval, requirements analysis and initial prototype |
| December 2026 | Process execution, supervision and initial isolation |
| January 2027 | Resource management and workload policies |
| February 2027 | Lifecycle management, integration and testing |
| March 2027 | Experimental evaluation, documentation and presentation |

## 10. Project Scope and Limitations

The initial implementation will target short-lived workloads on a single Linux host. Full container image management, production-grade security guarantees, complete OCI compliance and distributed orchestration are outside the mandatory academic scope.

These capabilities may be considered as future extensions.

## 11. Future Scope

Following successful completion of the core engine, the project may be extended to support rootless execution, standardized container runtime integration, remote workload execution, resource-aware scheduling and multi-server workload orchestration.

The long-term goal is to establish a foundation for an independent, extensible DevOps infrastructure platform.

## 12. Preliminary References

1. Open Container Initiative — Runtime Specification. https://specs.opencontainers.org/runtime-spec/
2. Linux Kernel Documentation — Control Group v2. https://docs.kernel.org/admin-guide/cgroup-v2.html
3. Youki — Rust Container Runtime. https://github.com/youki-dev/youki
4. Podman Documentation. https://docs.podman.io/
5. NsJail — Linux Process Isolation. https://github.com/google/nsjail
6. Bubblewrap — Unprivileged Sandboxing. https://github.com/containers/bubblewrap

*This concept proposal is preliminary and subject to modification based on university requirements and project supervisor feedback.*