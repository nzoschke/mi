---
title: Log
permalink: /log
---

# Log

```text
 ┌────────────────────────────────────┐ 
┌┤           Load Balancer            ├┐
│└────────────────────────────────────┘│
│┌─────────────────┐┌─────────────────┐│
││┌─────┐┌────────┐││     ┌─────┐     ││
│││web 1││worker 1│││     │web 2│     ││
││└─────┘└────────┘││     └─────┘     ││
││      VM 1       ││      VM 2       ││
│└─────────────────┘└─────────────────┘│
│              ┌────────┐              │
│              │Database│              │
│              └────────┘              │
│                 VPC                  │
└──────────────────────────────────────┘
 ┌──────┐┌─────┐┏━━━┓                   
 │Crypto││Image│┃Log┃                   
 └──────┘└─────┘┗━━━┛                   
```

A Log service provides a place to send text from an app's stdout and stderr streams, so events from more than one Container can be aggregated, tailed in real-time and searched for historical data.

We need Logs for an operator to get visibility into all the events happening in Containers and on VMs.

A Log service is a stand-alone service.
