---
title: "IIIF Design Patterns"
layout: spec
tags: [annex, presentation-api, image-api]
cssversion: 2
redirect_from:
  - /api/annex/notes/design_patterns.html
---

## Status of this Document
{:.no_toc}

This document is not subject to [IIIF's versioning semantics][iiif-semver]. Changes will be tracked within the document and its [internal change log][change-log]

**Authors:**

  * **[Michael Appleby](https://orcid.org/0000-0002-1266-298X)** [![ORCID iD](/img/orcid_16x16.png)](https://orcid.org/0000-0002-1266-298X), [_Yale University_](http://www.yale.edu/)
  * **[Tom Crane](https://orcid.org/0000-0003-1881-243X)** [![ORCID iD](/img/orcid_16x16.png)](https://orcid.org/0000-0003-1881-243X), [_Digirati_](http://digirati.com/)
  * **[Robert Sanderson](http://www.stanford.edu/~azaroth/)** [![ORCID iD](/img/orcid_16x16.png)](https://orcid.org/0000-0003-4441-6852), [_Stanford University_](http://www.stanford.edu/)
  * **[Jon Stroop](https://orcid.org/0000-0002-0367-1243)** [![ORCID iD](/img/orcid_16x16.png)](https://orcid.org/0000-0002-0367-1243), [_Princeton University Library_](https://library.princeton.edu/)
  * **[Simeon Warner](https://orcid.org/0000-0002-7970-7855)** [![ORCID iD](/img/orcid_16x16.png)](https://orcid.org/0000-0002-7970-7855), [_Cornell University_](https://www.cornell.edu/)
  {: .names}

{% include copyright2015.md %}

----

## Contents
{:.no_toc}
* Table of Discontent (will be replaced by macro)
{:toc}

## 1. Overview


## 2. Design Patterns Adopted

### Resource Orientation

We're REST and resources, not services.

### Linked Data

We conform to Linked Data standards, and follow the web architecture as defined by the W3C.

### JSON-LD First

But we focus on JSON-LD to make development easier.  The Context abstraction is important.

### Loose Coupling of IIIF APIs

APIs are loosely coupled rather than bound together.  Can implement presentation API without Image API.  

### Use Existing Standards Where Possible

We aim to be consistent with and use existing standards when possible.

### As Simple As Possible And No Simpler

### Define Success, Not Failure

We define what should be expected to work, not what shouldn't work.  Any pattern outside of those defined by the APIs is able to be used, keeping in mind future API extensions might make it inconsistent.

### Follow the IIIF Community Process

See [Community Process][process].

### Consider Implementation Requirements

Level 0 is important. Should be able to implement as flat files on disk.
Must not require expensive or complicated libraries.

### Use the Service Pattern for Extensions

See [Services][services].


## 5. Change Log

 | Date       | Description                                                         |
 | ---------- | ------------------------------------------------------------------- |
 | 2015-12-22 |  |

[change-log]: #change-log "Change Log"
[iiif-announce]: https://groups.google.com/forum/#!forum/iiif-announce "IIIF Email Announcement List"
[iiif-discuss]: https://groups.google.com/forum/#!forum/iiif-discuss "IIIF Email Discussion List"
[iiif-semver]: /api/annex/notes/semver/ "Versioning of APIs"
[rfc-2119]: https://www.ietf.org/rfc/rfc2119.txt "RFC 2119"
[spec-disclaimer]: /api/annex/notes/disclaimer/ "Specification Disclaimer"

[process]: /api/annex/notes/editors/#community-process
[services]: /api/annex/services/

{% include acronyms.md %}
