# Awesome-Application-Detection-n-Response

## Top Application Detection & Response (ADR) Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Runtime Application Security, In-App Attack Detection & Blocking, RASP Evolution, Code-Level Threat Visibility & Application-Layer Detection and Response*  

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Application Detection & Response (ADR)**. ADR (pioneered and popularized by Contrast Security as an evolution of RASP) embeds sensors inside running applications and APIs to observe code execution, data flow, and request handling—confirming real exploits rather than relying only on external traffic patterns—and supports detection, blocking, and response workflows.



**Examples** include Contrast Security (ADR / Protect), SentinelOne Singularity Cloud, CrowdStrike Falcon Cloud, Wiz Runtime, Apiiro, Ox Security, Aqua Security, Datadog AppSec / ASM, New Relic Security, and Dynatrace Application Security (the category leaders and adjacent runtime application security platforms).



**Open-source emphasis**: Full-featured commercial ADR/RASP platforms with deep language instrumentation, verified exploit detection, and enterprise response workflows dominate. Open-source options are more limited and include runtime security projects (eBPF/Falco-style), OpenRASP-style instrumentation, and emerging agent/runtime protection tools. This section lists every significant relevant project found.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Contrast Security (ADR / Protect)](https://www.contrastsecurity.com/)**  

  Pioneer of Application Detection and Response. Embeds lightweight sensors in the application runtime to confirm exploits at the code level, block attacks, and connect detection with vulnerability context and remediation guidance.



- **[Datadog AppSec / Application Security Management](https://www.datadoghq.com/)**  

  Runtime application security integrated with Datadog’s observability platform, providing attack detection, vulnerability insights, and response capabilities within the same monitoring stack.



- **[Dynatrace Application Security](https://www.dynatrace.com/)**  

  Runtime application security and vulnerability management built into the Dynatrace observability platform, leveraging deep code-level and runtime visibility.



- **[Aqua Security, Wiz Runtime](https://www.aquasec.com/)**  

  Cloud-native and runtime protection platforms offering workload, container, and application-layer runtime security and detection capabilities.



- **[SentinelOne Singularity Cloud, CrowdStrike Falcon Cloud](https://www.sentinelone.com/)**  

  Extended detection and response platforms with strong cloud workload and application runtime protection modules.



- **[Apiiro, Ox Security, New Relic Security](https://apiiro.com/)**  

  Application security platforms spanning code-to-runtime risk, attack-path analysis, and security observability for modern applications.



- **[Other commercial ADR / RASP / runtime application security platforms](https://www.contrastsecurity.com/)**  

  Solutions focused on in-app attack detection, blocking, and response for production applications and APIs.



## Open-Source GitHub Projects



- **[OpenRASP & similar runtime application protection projects](https://github.com/baidu/openrasp)**  

  Open-source Runtime Application Self-Protection style instrumentation that hooks into application runtimes to detect and block common attacks (SQL injection, XSS, etc.) from inside the process.



- **[Falco](https://github.com/falcosecurity/falco)**  

  Cloud-native runtime security project (CNCF) that uses eBPF/kernel instrumentation to detect anomalous behavior in containers, hosts, and Kubernetes—frequently used as a building block for workload and application runtime detection.



- **[eBPF-based runtime security tools](https://github.com/search?q=eBPF+runtime+security+OR+eBPF+application+security)**  

  Growing set of open projects leveraging eBPF for system-call and runtime behavior monitoring that can surface application-layer threats.



- **[OWASP & application security open tooling](https://github.com/OWASP)**  

  OWASP projects related to runtime protection concepts, security testing, and defensive libraries that complement ADR-style approaches.



- **[Agent / AI runtime protection open projects](https://github.com/search?q=AI+agent+runtime+security+OR+agent+detection+response)**  

  Emerging open-source tools focused on monitoring and controlling AI agents at runtime (tool use, prompt injection, policy enforcement)—a newer adjacent category sometimes also labeled ADR.



- **[RASP research & academic prototypes](https://github.com/search?q=RASP+OR+%22runtime+application+self-protection%22)**  

  Community and research implementations exploring in-app instrumentation and attack detection techniques.



- **[WAFs & ModSecurity-style open engines](https://github.com/owasp-modsecurity/ModSecurity)**  

  Open web application firewall engines that provide complementary (network/edge) detection and can be paired with runtime sensors.



- **[Tracing & observability open stacks used for security](https://github.com/search?q=OpenTelemetry+security+OR+application+tracing)**  

  OpenTelemetry and related tracing tools that some teams extend for security-relevant runtime signals.



### Additional Strong Open-Source Options



- **In-app instrumentation**: OpenRASP-style projects for classic RASP behavior inside application processes.

- **Kernel / container runtime**: Falco and eBPF tools for workload-level detection that can catch application-related anomalies.

- **Composable defense**: Open RASP + Falco + SIEM/alerting for layered runtime visibility.

- **Emerging agent security**: Open tools specifically targeting AI agent runtime behavior.

- Full commercial ADR platforms remain significantly more mature for language coverage, verified exploit confirmation, low false positives, and integrated response workflows.



**Frameworks for building custom systems**:  

There is no complete open-source equivalent to commercial ADR platforms such as Contrast ADR that combine deep language instrumentation, verified exploit detection, blocking, and response orchestration at enterprise scale.  

The strongest open building blocks are **OpenRASP**-style instrumentation, **Falco**/eBPF runtime security, and emerging agent-protection projects.  

Commercial platforms (Contrast, Datadog AppSec, Dynatrace, Aqua, Wiz, SentinelOne, CrowdStrike, etc.) deliver production-grade sensors, language support, low-noise detection, and SOC integration.  

Many organizations use commercial ADR/RASP for critical applications and open runtime tools (Falco, eBPF) for broader workload coverage. Fully open stacks require significant custom development and validation for production use.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Runtime application security sensors run inside or alongside production applications. Incorrect configuration can impact performance, availability, or create false confidence. Always test thoroughly and maintain defense-in-depth (secure coding, WAF, network controls, etc.).

- Open-source runtime tools offer transparency but generally lack the language coverage, verified detection accuracy, and enterprise support of commercial ADR platforms. Evaluate performance overhead, false-positive rates, and operational readiness carefully before production deployment.



---



**Made for AppSec engineers, SecOps teams, platform security, and developers protecting applications at runtime.**  

Let's expand open runtime detection options while recognizing the depth, accuracy, and response capabilities that leading commercial Application Detection & Response platforms deliver.

