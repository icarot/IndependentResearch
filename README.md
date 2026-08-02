# Independent Research
This repository has the goal to centralize all independent research performed by me during my free time, the objective is to study and contribute with the infosec community by finding possible low hanging fruit vulnerabilities still existing on important open source solutions/applications.

## Apache Kyuubi: Unrestricted access via Kyuubi engine-ui proxy (CVE-2026-23904)
Kyuubi Engine UI proxy accepts a host and port from the request path and proxies HTTP requests to that destination. A remote requester with network access to the proxy can cause the Kyuubi server to send HTTP requests to arbitrary reachable hosts, resulting in SSRF or open-proxy behavior. This issue affects Apache Kyuubi: from 1.8.0 before 1.12.0. Users are recommended to upgrade to version 1.12.0, which disables the proxy by default. To restore proxied Engine UI, set kyuubi.frontend.rest.engine.ui.proxy.enabled=true and configure allowed target hosts with kyuubi.frontend.rest.engine.ui.proxy.hosts.

- https://lists.apache.org/thread/ps79fcfx49ox9kwgztc5t5bw0tyhck9m
- https://www.cve.org/CVERecord?id=CVE-2026-23904

## Apache Superset: When the default configuration turns you “Super(up)set”? (Article)
- https://medium.com/@icarot/when-the-default-configuration-turns-you-super-up-set-b7febcd9b9ea
- https://lists.apache.org/thread/pydlykgbsb9bjlnt8g789pjw7k8rt2ht
- https://github.com/icarot/superUpset

## Apache HertzBeat: Exposure sensitive token via http GET method with query string (CVE-2024-45791)
Exposure of Sensitive Information to an Unauthorized Actor vulnerability in Apache HertzBeat. This issue affects Apache HertzBeat: before 1.6.1. Users are recommended to upgrade to version 1.6.1, which fixes the issue.

- https://lists.apache.org/thread/lvsczrp8kdynppmzyxtkh4ord4gpw1ph
- https://www.cve.org/CVERecord?id=CVE-2024-45791
