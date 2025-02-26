---
title: Bug Check 0x168 CLUSTER_CSV_STATE_TRANSITION_TIMEOUT_LIVEDUMP
description: The CLUSTER_CSV_STATE_TRANSITION_TIMEOUT_LIVEDUMP bug check has a value of 0x00000168. This indicates that a Cluster Shared Volume state transition took too long.
keywords: ["Bug Check 0x168 CLUSTER_CSV_STATE_TRANSITION_TIMEOUT_LIVEDUMP", "CLUSTER_CSV_STATE_TRANSITION_TIMEOUT_LIVEDUMP"]
ms.date: 01/03/2019
topic_type:
- apiref
api_name:
- CLUSTER_CSV_STATE_TRANSITION_TIMEOUT_LIVEDUMP
api_type:
- NA
---

# Bug Check 0x168: CLUSTER\_CSV\_STATE\_TRANSITION\_TIMEOUT\_LIVEDUMP

The CLUSTER\_CSV\_STATE\_TRANSITION\_TIMEOUT\_LIVEDUMP bug check has a value of 0x00000168. This indicates that a Cluster Shared Volume state transition took too long.


> [!IMPORTANT]
> This topic is for programmers. If you are a customer who has received a blue screen error code while using your computer, see [Troubleshoot blue screen errors](https://www.windows.com/stopcode).



## CLUSTER\_CSV\_STATE\_TRANSITION\_TIMEOUT\_LIVEDUMP Parameters

|Parameter|Description|
|--- |--- |
|1| Cluster Service PID.|
|2| CSV target state Id - listed below. |
|3| Reserved |
|4| Reserved |


**CSV target state Id**

0  Waiting for volume to transition to the Init state. 

1  Waiting for volume to transition to the Paused state. 

2  Waiting for volume to transition to the Draining state. 

3  Waiting for volume to transition to the Set-Down-Level state. 

4  Waiting for volume to transition to the Active state.


## Cause

A Cluster Shared Volume state transition took too long. The system generated a live dump for analysis of the delay.

(This code can never be used for a real bugcheck.)

## Resolution
 

## See Also-

[Troubleshooting Hangs Using Live Dump (Blog)](https://techcommunity.microsoft.com/t5/Failover-Clustering/bg-p/FailoverClustering)

[Bug Check Code Reference](bug-check-code-reference2.md)




