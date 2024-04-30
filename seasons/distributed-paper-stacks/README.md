
# Reading Stacks Season 2: Distributed Paper Stacks

In this season of Reading Stacks, we will host 4 episodes on different topics in distributed systems. In each episode, we will base our discussions on a fundamental paper in the field, and augment the discussion with interactive demos, tutorials, use cases of the concepts in real-world systems, and more.

The four episodes are:

(1) Distributed Queues by Can Toraman *(May 15, 2024)*
(2) Distributed Key-Value Stores by Ozan Sazak *(May 29, 2024)*
(3) Realtime State Sharing with CRDTs by Alperen Keles and Ozan Akin *(June 12, 2024)*
(4) Latency in Distributed Systems by Yigit Varli *(June 26, 2024)*

Below, you can find the abstracts for each episode.

## Episode 1: Distributed Queues

**Host:** Can Toraman  
**Date:** May 15, 2024

<details>
<summary>
Click to see the abstract
</summary>
In this episode of Paper Stacks, Can Toraman will be discussing Achieving Task-Based Scheduling in Low-Latency Distributed Priority Queues.

In modern distributed systems, managing the queue efficiently is crucial for performance and responsiveness. Especially in multi-tenant environments, prioritizing different tasks (based on customer, task type, etc) is crucial. Yet, this area is still not highly explored, as many companies solve it by using different queues. Well, are more optimal ways, and how are they achievable in a distributed setting?

Distributed priority queues are still not highly explored in the academic environment, so will base our discussions on different theoretical and practical perspectives used in the industry:

- Timestone, Netflix’s distributed queue used in its encoding service 
- ⁠B4, Google’s Wide Area Network to support requests from both GCP and Google applications.
- ⁠Facebook’s FOQS to support horizontal scaling and multi-tenant environments
- ⁠QPID: A Distributed Priority Queue with Item Locality

Links:

- Timestone: [https://netflixtechblog.com/timestone-netflixs-high-throughput-low-latency-priority-queueing-system-with-built-in-support-1abf249ba95f](https://netflixtechblog.com/timestone-netflixs-high-throughput-low-latency-priority-queueing-system-with-built-in-support-1abf249ba95f)
- B4: [https://research.google/pubs/b4-and-after-managing-hierarchy-partitioning-and-asymmetry-for-availability-and-scale-in-googles-software-defined-wan/](https://research.google/pubs/b4-and-after-managing-hierarchy-partitioning-and-asymmetry-for-availability-and-scale-in-googles-software-defined-wan/)
- FOQS: [https://engineering.fb.com/2021/02/22/production-engineering/foqs-scaling-a-distributed-priority-queue/](https://engineering.fb.com/2021/02/22/production-engineering/foqs-scaling-a-distributed-priority-queue/)
- QPID: [https://ieeexplore.ieee.org/document/4725152](https://ieeexplore.ieee.org/document/4725152)
</details>

## Episode 2: Distributed Key-Value Stores

**Host:** Ozan Sazak  
**Date:** May 29, 2024

<details>
<summary>
Click to see the abstract
</summary>
In this episode of Paper Stacks, Ozan Sazak will explore the internals of Amazon Dynamo, a highly available and scalable key-value store.

Dynamo, developed for Amazon’s critical services, addressed the internal needs of Amazon using techniques such as consistent hashing, quorum-like techniques, and eventual consistency.

We’ll dive into the 2007 Dynamo paper, discuss the internals of the Dynamo, and the design decisions between the parts such as partitioning and replication.

Paper Link: [https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf](https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf)
</details>

## Episode 3: Realtime State Sharing with CRDTs

**Host:** Alperen Keles and Ozan Akin  
**Date:** June 12, 2024

<details>
<summary>
Click to see the abstract
</summary>
In this episode of Paper Stacks, Alperen Keles and Ozan Akin will be discussing
Real-Time Distributed State Sharing for Collaborative Applications using Conflict-Free
Replicated Data Types(CRDTs).

Sharing state between multiple servers and clients is extremely common today. When
multiple users make concurrent updates on a shared data structure, the applications need 
conflict resolution strategies to ensure all users agree on the final state. 

CRDTs are one such mechanism for handling distributed state; the differentiating factors
for CRDTs are (1) they don't need a central server, (2) they are highly fault-tolerant, allowing
users to work offline, and sync their work at arbitrary intervals.

Within the episode, we will base our discussions on the 2011 paper by Marc Shapiro, discuss the 
usage of CRDTs in collaborative text editing in Zed Code Editor, collaborative canvases such as
Excalidraw and Figma, and provide live demos on the internal workings of CRDTs.

Paper Link: [https://inria.hal.science/inria-00555588/document](https://inria.hal.science/inria-00555588/document)
</details>

## Episode 4: Tail Latency in Distributed Systems

**Host:** Yigit Varli  
**Date:** June 26, 2024

<details>
<summary>
Click to see the abstract
</summary>

In this episode of Paper Stacks, Yigit Varli will be discussing the challenges of
optimizing tail latencies in large-scale distributed systems.

Distributed systems tend to serve a diverse set of users at geographically varying locations, with
heterogeneous loads and requirements. Classically, such systems have optimized for “average latency”,
which resulted in very high latency for a small subset of users, the so-called tail.

In this episode, we will dive into 'The Tail at Scale' by Jeffrey Dean and Luiz André Barroso from Google,
where we will explore system designs and techniques to handle high loads, ensuring smoother operation and
improved user experience.

Paper Link: [https://dl.acm.org/doi/pdf/10.1145/2408776.2408794](https://dl.acm.org/doi/pdf/10.1145/2408776.2408794)
</details>