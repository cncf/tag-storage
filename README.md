# CNCF SIG Storage

## Meetings

The Storage SIG meets on the 2nd and 4th Wednesday of every month at 8AM PT (USA Pacific):

Join from PC, Mac, Linux, iOS or Android: https://zoom.us/my/cncfstoragewg

Or iPhone one-tap (US Toll): +16465588656,158580155# or +14086380968,158580155#

Or Telephone: Dial: +1 646 558 8656 (US Toll) or +1 408 638 0968 (US Toll) Meeting ID: 158 580 155 International numbers available: https://zoom.us/zoomconference?m=0gvI03dCdRnx6WENPzdNhioORGmhVwYo

## Mailing list and minutes

Mailing lists: https://groups.google.com/forum/#!forum/cncf-wg-storage
Meeting minutes are recorded here: https://goo.gl/wRqerO


## Areas Considered In Scope

Storage systems and approaches suitable for and commonly used in
[modern cloud-native
environments](https://github.com/cncf/toc/blob/master/DEFINITION.md):

*   especially where these differ significantly from storage systems
    and approaches previously commonly used in traditional enterprise
    data center environments,
*   and which are not already adequately covered by other groups within the CNCF (see below).  
*   storage includes block stores, file systems, object stores, databases, key-value stores, and related caching mechanisms. 

We strive to understand the fundamental characteristics of different
storage approaches with respect to availability, scalability,
performance, durability, consistency, ease-of-use, cost and
operational complexity; and relate these to their suitability to
various cloud-native use cases. This is covered in more detail in the
[CNCF Storage Landscape White Paper](
http://bit.ly/cncf-storage-whitepaper).

## Areas Considered Out Of Scope

Anything not considered in scope above (:-)).  See also “Interfaces
with Related Groups” below.

Examples include:

*   Details of general-purpose low-level storage media like magnetic
    hard disks, solid-state storage devices, non-volatile memory, etc
    (which tend not to be very different irrespective of whether or
    not they’re being used in a cloud-native environment).
*   General authentication, authorization, accounting, auditing etc
    (even though these clearly apply to storage systems too) - because
    AAA etc is clearly the domain of the CNCF Security SIG.
*   Standardizing container storage interfaces - this is the domain of CSI.
*   Defining storage abstraction APIs for container orchestrators -
    these are the domains of the Storage SIGs specific to each
    orchestrator, e.g. Kubernetes Storage SIG.

## SIG Mission Statement

To enable widespread and successful storage of persistent state in
cloud-native environments through:

1. Providing valuable and objective information to the TOC, End Users
   and Projects of the CNCF regarding areas considered in scope (see
   above).
2. Collaborating effectively with other related groups (see below).
3. Helping to maintain the continued health of CNCF Storage Projects
   (see below)
4. Identifying and filling gaps in the landscape of CNCF Storage
   Projects.

## Current CNCF Storage Projects

1. TiKV
2. etcd
3. Vitess
4. Rook
5. OpenEBS

## Interfaces With Other Related Groups

*   **Kubernetes Storage SIG** - is focussed towards
    Kubernetes-specific storage abstractions, interfaces, and
    implementations of these interfaces.  We maintain close
    communication with this Kubernetes SIG, with several individuals
    actively involved in both.  Our aim is to avoid unnecessary
    duplication of effort by the two groups, and maintain clear an
    consistent messaging by the two groups to our end user community
    and projects.
*   **CSI** - is focussed on defining an industry standard “Container
    Storage Interface” (CSI) that will enable storage vendors to
    develop a plugin once and have it work across a number of
    container orchestration systems.  Again, we maintain close
    communication with this group, and avoid unnecessary duplication
    of effort and inconsistent messaging wherever possible.
*   **CNCF Security SIG** - works on the more general area of
    cloud-native security including authentication, authorization,
    encryption, accounting, auditing and related topics.  We defer as
    much as possible to this group to deal with general
    security-related issues, and liaise closely with them on how to
    deal with storage-specific security areas where these arise.
*   **CNCF Apps SIG** (not yet fully formed) - will be focussed on the
    development, deployment, operation and testing of cloud-native
    applications.  We collaborate with this SIG where this pertains to
    Storage.
*   **K8s Apps SIG** - has done some work on how Kubernetes apps use
    storage, as well as how storage systems (including databases) may
    be deployed on Kubernetes .  We collaborate with Apps SIG and make
    sure that important topics are well covered.
*   **[Kubernetes Service Catalog SIG](https://github.com/kubernetes/community/tree/master/sig-service-catalog)**-
    works on enabling external managed software offerings such as
    datastore services offered by public cloud providers.

## Operating Model

This SIG follows the [standard operating
guidelines](https://github.com/cncf/toc/blob/master/sigs/cncf-sigs.md#operating-model)
provided by the TOC unless otherwise stated here.

**Current TOC Liaison:** Xiang Li

**[Proposed] Co-Chairs:** Alex Chircop, Quinton Hoole, “One Other TBD”

**[Proposed] Tech Leads:** Saad Ali, Xing Yang, Sugu Sougoumarane
