# CNCF Storage TAG

## Meetings

The Storage Technical Advisory Group meets on the 2nd and 4th Wednesday of every month at 8AM PT (USA Pacific):

Join from PC, Mac, Linux, iOS or Android: https://zoom.us/j/2920471159?pwd=em1JbE44MktjZE4vbnJtUUFQcGZwdz09

Or iPhone one-tap (US Toll): +16465588656,158580155# or +14086380968,158580155#

Or Telephone: Dial: +1 646 558 8656 (US Toll) or +1 408 638 0968 (US Toll) Meeting ID: 158 580 155 International numbers available: https://zoom.us/zoomconference?m=0gvI03dCdRnx6WENPzdNhioORGmhVwYo

## Mailing list and minutes

Mailing list: https://lists.cncf.io/g/cncf-tag-storage 

(note: the old WG mailing list is here: https://groups.google.com/forum/#!forum/cncf-wg-storage)

Meeting minutes are recorded here: https://bit.ly/cncf-storage-sig-minutes


## CNCF Storage TAG Charter

The charter is available here: https://github.com/cncf/tag-storage/blob/master/storage-charter.md


## CNCF Storage Landscape Whitepaper

The whitepaper documents the storage landscape by clarifying the terminology used in the storage space including:

- The attributes of a storage system such that an end-user can understand the appropriate capabilities that might be required by an application or architectural pattern.
- The layers in a storage solution (or service) with a focus on terminology and how they impact the defined attributes covering the container, orchestrator, transport, topology, virtual/physical, data protection, data services and the non-volatile layers.
- The data access interfaces in terms of volume (including block, file system and shared file system) and application API (including object, KV and database) as high level groupings.
- Separate sections with further detail on Block Storage, File systems, Object Storage and Key Value Stores.
- The management interfaces needed to orchestrate the storage layers to facilitate composability, dynamic provisioning and self service management.

The whitepaper is available here: https://bit.ly/cncf-storage-whitepaperV2

PDF copy is available in the repo here: https://github.com/cncf/tag-storage/blob/master/CNCF%20Storage%20Whitepaper%20V2.pdf


## Cloud Native Disaster Recovery Whitepaper

This document covers how disaster recovery is implemented in cloud native environments and covers:

- Definition of Cloud Native Disaster Recovery (CNDR) including failure domains, HA & DR
- CAP theorem: Consistency, Availability, Network Partitioning 
- Anatomy of Distributed Stateful workloads: Replicas, Shards, API Layer, Storage Layer
- Consensus Protocols: Paxos, Raft, 2PC, 3PC
- CNDR Reference Architectures

The document is available here: https://bit.ly/cncf-cloud-native-DR

PDF copy is availaber in the repo [her](https://github.com/cncf/tag-storage/blob/master/cloud-native-disaster-recovery-whitepaper/Cloud%20Native%20Disaster%20Recovery%20V1.pdf).

## Data on Kubernetes Whitepaper - Database Patterns

This document describes patterns of running data on Kubernetes. This is a collaboration between TAG Storage and [Data on Kubernetes Community](https://dok.community/) (DoKC). In this version of the whitepaper, we are focusing on database workloads. It covers the following:

- Attributes of a storage system and how they affect running data in Kubernetes
- Running data inside vs outside of Kubernetes
- Common Kubernetes patterns and features used when running data on Kubernetes
- Observability
- Security
- Day 2 operations

The document is available [here](data-on-kubernetes-whitepaper/data-on-kubernetes-whitepaper-databases.md).

## Current CNCF Storage Projects

### Graduated Projects

- [etcd](https://github.com/etcd-io/etcd)
- [Harbor](https://github.com/goharbor/harbor)
- [Rook](https://github.com/rook/rook)
- [TiKV](https://github.com/tikv/tikv)
- [Vitess](https://github.com/vitessio/vitess)

### Incubating Projects

- [CubeFS](https://github.com/cubefs/cubefs)
- [Dragonfly](https://github.com/dragonflyoss/Dragonfly)
- [Longhorn](https://github.com/longhorn/longhorn)

### Sandbox Projects

- [Carina](https://github.com/carina-io/carina)
- [Curve](https://github.com/opencurve/curve)
- [Hwameistor](https://github.com/hwameistor/hwameistor)
- [K8up](https://github.com/k8up-io/k8up)
- [OpenEBS](https://github.com/openebs)
- [Pravega](https://github.com/pravega/pravega)
- [Piraeus](https://github.com/piraeusdatastore/piraeus)
- [Vineyard](https://github.com/v6d-io/v6d)
- [Xline](https://github.com/xline-kv/Xline)(onboarding)

## Operating Model

This TAG follows the [standard operating
guidelines](https://github.com/cncf/toc/blob/main/tags/README.md#operating-model)
provided by the TOC unless otherwise stated here.

**Current TOC Liaison:** Nikhita Raghunath, Matt Farina

**Co-Chairs:** Alex Chircop, Xing Yang, Raffaele Spazzoli

**Tech Leads:** Luis Pabon, Sheng Yang, Nick Connolly

**Other named roles:** None at present; will be identified and staffed as needed.
