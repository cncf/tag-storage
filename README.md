# wg-storage

CNCF Storage Working Group

## Goals

Explore cloud native storage technology and concepts.

## Why is storage important to cloud native

- There’s no such thing as a stateless architecture, applications store state somewhere
- Storage further enables specific cloud native patterns
- Interoperating with storage increases cloud native’s relevance and leads to better applications

## Mission statement

In support of cloud native computing, the SWG intends to enable a thriving storage eco-system that is vendor and platform neutral and interoperable for applications

## Responsibilities

- Make sense of storage eco-system supporting cloud native environments
- Review storage projects
- Assist storage projects in TOC project nomination process

## Governance

The storage working group is an open group of community members with a leading representative as defined by the CNCF TOC (Ben Hindman). It meets regularly and members provide input and opinions about storage topics. Leadership makes decisions on SWG perspectives to be delivered to the TOC. 

## What is Cloud Native Storage
Cloud Native Storage is a classification for storage resources that are interoperable for applications in cloud native environments. It is not necessarily a cloud native system itself, but supports decoupling of storage services from applications. Interoperability is possible through standard storage interfaces. These resources are reliable, consumed on-demand, and self-provisioned. Resources can be elastic in both capacity and performance and utilization is measured to enable optimal and efficient use. The consumption experience is completely seamless where operations are transparent. 

Cloud Native Storage is not limited and specific to an access method or data structure. In fact numerous types of storage can all be classified using this application view. This is important to ensure that the evolving interaction of the application with storage is consistent. The shift from the monolithic application includes the storage of files and blocks in addition to more efficient and distributed higher-level structured data services. Cloud Native Storage supports a progressive view and not exclusive to volumes, objects, sql and nosql, keys and values, queues, time-series, logs, and records.

In summary,
- Consumption experience is seamless and operations are transparent
  - Supports decoupling of storage services from applications
- Resources consumed on-demand and self-provisioned
  - Reliable and elastic in both capacity and performance
- Seemingly unlimited resources that are measured to ensure optimal and efficient use
  - Interoperability occurs through standard interfaces
- CNS itself does NOT define a type of storage

## Technical Scope

Scope of SWG includes a progressive view of storage as defined by Cloud Native Storage; will review different types of storage (blocks, files, object, sql, nosql, key value, queues, time-series, logs, etc.) and different components in landscapes (interfaces, frameworks, tools, plugins, providers).


## Initiatives and Interesting Projects

### Container Storage Interface (CSI)

A project that aims to define an industry standard “container storage interface” (CSI). This interface would enable a storage vendors to write a driver once and have it work across a number of container orchestration (CO) systems

See this repo for more information: https://github.com/container-storage-interface/spec

## Members and Mailing List

https://groups.google.com/forum/#!forum/cncf-wg-storage

## Meeting Minutes

The Storage Working Group meets on the 2nd and 4th Wednesday of every month at 8AM PT (USA Pacific):

Join from PC, Mac, Linux, iOS or Android: https://zoom.us/j/158580155

Or iPhone one-tap (US Toll):  +16465588656,158580155# or +14086380968,158580155#

Or Telephone:
    Dial: +1 646 558 8656 (US Toll) or +1 408 638 0968 (US Toll)
    Meeting ID: 158 580 155
    International numbers available: https://zoom.us/zoomconference?m=0gvI03dCdRnx6WENPzdNhioORGmhVwYo
    
NOTE: Please use *6 to mute/un-mute your phone during the call.
    
Here is a public Google calendar so you can add the meetings to your calendar: https://goo.gl/eyutah

Here is a link to a World Time Zone Converter here:  http://www.thetimezoneconverter.com/?t=8:00%20a.m.%20&tz=San%20Francisco&


### Meeting Recordings

Meeting minutes are recorded here: https://goo.gl/wRqerO

Recordings of meeting calls:
* [6/9/2017](https://youtu.be/qAw3y6rdRbs)
* [7/18/2017](https://zoom.us/recording/play/zIMhdwzItxsEEUvFk7gYxTOqShJoOjrPcFcV0mHm9N-Rf1Ql6fypw59APZBsjmmG)
* [8/8/2017](https://www.youtube.com/watch?v=d_zQFASkssU)
* [9/20/2017](https://www.youtube.com/watch?v=PjB4qXeN-ks)
