---
title: Object Store NAS Gateway Using MinIO
authors:
  - "@lpabon"
owning-sig: sig-storage
reviewers:
  - TBD
approvers:
  - TBD
creation-date: 2019-11-13
last-updated: yyyy-mm-dd
status: deferred|rejected|withdrawn|replaced
---

# Use Case: Object Store NAS Gateway Using MinIO

This document describes a recommended storage model for deploying an
object store NAS gateway using [MinIO](https://min.io/). This model can be
used when there is a requirement to access files from both
[shared file system](https://docs.google.com/document/d/1Cek8jJ2SPt4xx7Tnx7ih_m4DxzSimj_w26qYHnfrrRQ/edit#heading=h.pbmybfjw6u9v)
and
[object store](https://docs.google.com/document/d/1Cek8jJ2SPt4xx7Tnx7ih_m4DxzSimj_w26qYHnfrrRQ/edit#heading=h.1y7m8ig3tq5o)
interfaces.

<!-- This table is created by the VSCode Markdown Addon -->
- [Use Case: Object Store NAS Gateway Using MinIO](#use-case-object-store-nas-gateway-using-minio)
  - [Goals](#goals)
  - [Non-goals](#non-goals)
  - [Storage Landscape Summary](#storage-landscape-summary)
    - [Storage Stacks](#storage-stacks)
    - [Block Stores](#block-stores)
    - [File Systems](#file-systems)
    - [Other Stores](#other-stores)
  - [References](#references)

## Goals

- Save files as object over the object store interface
- Load files over shared file system interface

## Non-goals

- A step-by-step model of how to accomplish this deployment
- Describe storage scalibility

## Storage Landscape Summary

### [Storage Stacks](https://docs.google.com/document/d/1Cek8jJ2SPt4xx7Tnx7ih_m4DxzSimj_w26qYHnfrrRQ/edit#heading=h.baxsjwj26tbn)

<!-- 
    Alt-Shift-F in VSCode Markdown Addon to automatically size table width.
    Not necessary
-->

| Storage Stack  |    Recommended     | Notes                                                          |
| -------------- | :----------------: | -------------------------------------------------------------- |
| Centralised    | :heavy_check_mark: | Shared storage is required                                     |
| Distributed    | :heavy_check_mark:  | Shared storage is required                                     |
| Sharded        | :heavy_check_mark: | A shared centralised or distributed storage system is required |
| Hyperconverged | :heavy_check_mark: | Shared storage is required                                     |

### [Block Stores](https://docs.google.com/document/d/1Cek8jJ2SPt4xx7Tnx7ih_m4DxzSimj_w26qYHnfrrRQ/edit#heading=h.tvi9orfkisq7)

All of the following block stores will require a file system on top
of the block device and a service to share the volume to other systems.
It is also highly recommended that the block volume has an appropriate
[durability](https://docs.google.com/document/d/1Cek8jJ2SPt4xx7Tnx7ih_m4DxzSimj_w26qYHnfrrRQ/edit#heading=h.dh09gq1vn6a7)
model.

| Block Stores |    Recommended     | Notes                                                                                                                                                          |
| ------------ | :----------------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Local        | :heavy_check_mark: |                                                                                                                                                                |
| Remote       | :heavy_check_mark: | It will also provide more application up-time since it can connect and reconnect from one node to another, for example, in a virtual machine or in Kubernetes. |
| Distributed  | :heavy_check_mark: |                                                                                                                                                                |

### [File Systems](https://docs.google.com/document/d/1Cek8jJ2SPt4xx7Tnx7ih_m4DxzSimj_w26qYHnfrrRQ/edit#heading=h.ysbf15wa3ar5)

It is highly recommended that the file system volume has an appropriate
[durability](https://docs.google.com/document/d/1Cek8jJ2SPt4xx7Tnx7ih_m4DxzSimj_w26qYHnfrrRQ/edit#heading=h.dh09gq1vn6a7)
model.

| File Systems |    Recommended     | Notes                                                                                                                                                                                                                                 |
| ------------ | :----------------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Local        | :heavy_check_mark: | Will require a service to allow clients to access the file system over the network                                                                                                                                                    |
| Remote       | :heavy_check_mark: | Service to allow clients to access already provided by storage system. It will also provide more application up-time since it can connect and reconnect from one node to another, for example, in a virtual machine or in Kubernetes. |
| Distributed  | :heavy_check_mark: |                                                                                                                                                                                                                                       |

### [Other Stores](https://docs.google.com/document/d/1Cek8jJ2SPt4xx7Tnx7ih_m4DxzSimj_w26qYHnfrrRQ/edit#heading=h.lrlu2fsu69n8)

The following stores cannot be used in this use case.

| Stores          | Recommended | Notes |
| --------------- | :---------: | ----- |
| Object Store    |     :x:     |       |
| Key-Value Store |     :x:     |       |

## References

- [MinIO NAS Gateway](https://docs.min.io/docs/minio-gateway-for-nas.html)
