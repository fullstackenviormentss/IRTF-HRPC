---
title: Human Rights Protocol Considerations - Research Report
docname: draft-doria-hrpc-report
date: 2015-10-11
category: info

ipr: trust200902
 
area: IRTF
workgroup: Human Rights Protocol Consideration RG
keyword: Internet-Draft
stand_alone: yes
pi:
  rfcedstyle: yes
  toc: yes
  tocindent: yes
  sortrefs: yes
  symrefs: yes
  strict: yes
  comments: yes
  inline: yes
  text-list-symbols: -o*+

author:
-
  ins: A. Doria
  name: Avri Doria
  org: Technicalities
  email: avri@acm.org

normative:

informative:
  RFC1958:
  RFC1984:
  RFC2026:
  RFC2639:
  RFC2919:
  RFC3365:
  RFC5890:
  RFC5891:
  RFC5892:
  RFC5893:
  RFC6162:
  RFC6783:
  RFC6973:
  RFC7230:
  RFC7231:
  RFC7232:
  RFC7234:
  RFC7235:
  RFC7236:
  RFC7237:
  RFC7258:
  UDHR:
    title: The Universal Declaration of Human Rights
    date: 1948
    author:
      org: United Nations General Assembly
    target: http://www.un.org/en/documents/udhr/
 
  HRPC-GLOSSARY:
    title: Human Rights Protocol Considerations Glossary
    date: 2015
    author:
      - ins: N. ten Oever
      - ins: A. Doria
      - ins: D. K. Gillmor
    target: https://www.ietf.org/id/draft-dkg-hrpc-glossary-00.txt
 
  HRPC-Method:
    title: Human Rights Protocol Considerations Methodology
    date: 2015
    author:
      - ins: J. Varon
      - ins: C. Cath
    target: https://www.ietf.org/id/draft-varon-hrpc-methodology-00.txt

  Cath:
    title: A case study of codeing rights
    date: 2015
    author:
       - ins: C. Cath

  Clark:    
    title: The Design Philosophy of the DARPA Internet Protocols
    author:
      - ins: D. Clark
    seriesinfo: Proc SIGCOMM 88, ACM CCR Vol 18, Number 4, August
        1988, pp. 106-114.
    date: 1988

  Blumenthal:
    title: Rethinking the design of the Internet The end-to-end arguments vs. the brave new world
    author:
       - ins: M. Blumenthal
       - ins: D.D. Clark
    seriesinfo: ACM Transactions on Internet Technology, Vol. 1, No. 1, August 2001, pp 70-109.
    date: 2001

 
  Liddicoat:
    title: Human Rights and Internet Protocols
    author:
       - ins: J. Liddicoat
       - ins: A. Doria
    target: https://www.apc.org/en/pubs/human-rights-and-internet-protocols-comparing-proc
   
  Denardis:
    title: Protocol Politics
    author:
      - ins: L. Denardis
    date: 2013
   
  Post:
    title: Internet Infrastructure and IP Censorship
    author:
      - ins: D. Post
    date: 2015
    target:  http://www.ipjustice.org/digital-rights/internet-infrastructure-and-ip-censorship-bydavid-post/

  Zittrain:
    title: The Future of the Internet And How to Stop It
    date: 2008
    author:
      - ins: J. Zittrain

--- abstract

This document present an overview of the project to map engineering concepts at the protocol level that may be related to promotion and protection of the freedom of expression and association.

This first draft is intended to provide the framework for reporting on the study, initial results and basic considerations. At a later stage it will fold in the work being done in the Methodology and Glossary drafts as well as the work being done in the case studies. It also folds in some of the text included in the original proposal for the HRPC.

Discussion on this draft at: hrpc@irtf.org // https://www.irtf.org/mailman/admindb/hrpc

--- middle


Background
============

The recognition that human rights have a role in Internet policies has become part of the general discourse.  Several reports from former United Nations (UN) Special Rapporteur on the promotion and protection of the right to freedom of opinion and expression, Frank La Rue, have made such relation explicit, which lead to the approval of the landmark resolution "on the promotion, protection and enjoyment of human rights on the Internet" at the UN Human Rights Council (HRC).  And, more recently, to the resolution "The right to privacy in the digital age" at the UN General Assembly.  The NETmundial outcome document affirms that human rights, as reflected in the Universal Declaration of Human Rights {{UDHR}}, should underpin Internet governance principles.

Nevertheless, the direct relation between Internet Standards and human rights is still something to be explored and more clearly demonstrated.

Concerns for freedom of expression and association were a strong part of the world-view of the community involved in developing the first Internet protocols.  Apparently, by intention or by coincidence, the Internet was designed with freedom and openness of communications as core values.  But as the scale and the commercialization of the
Internet has grown, the influence of such world-views had to compete with other values, such as ease of development and cost. The purpose of this research is to discover and document the consideration involved in taking human rights into account when creating protocols.

In a manner similar to the work done for RFC 6973 {{RFC6973}} on Privacy Consideration Guidelines, the premise of this research is that some standards and protocols can solidify, enable or threaten user rights.

As stated in RFC 1958 {{RFC1958}}, the Internet aims to be the global network of networks that provides unfettered connectivity to all users at all times and for any content.  Open, secure and reliable  connectivity is essential for rights such as freedom of expression and freedom of association, as defined in the Universal Declaration   of Human Rights {{UDHR}}.  Therefore, considering connectivity as the ultimate objective of the Internet, this makes a clear case that the   Internet is not only an enabler of human rights, but that human rights lie at the basis of, and are ingrained in, the architecture of   the network.

An essential part of maintaining the Internet as a tool for communication and connectivity is security.  Indeed, "development of security mechanisms is seen as a key factor in the future growth of  the Internet as a motor for international commerce and communication"   RFC 1984 [RFC1984] and according to the Danvers Doctrine RFC 3365  {{RFC3365}}, there is an overwhelming consensus in the IETF that the  best security should be used and standardized.

In RFC 1984 {{RFC1984}}, the Internet Architecture Board (IAB) and the  Internet Engineering Steering Group (IESG), the bodies which oversee   architecture and standards for the Internet, expressed: "concern by  the need for increased protection of international commercial   transactions on the Internet, and by the need to offer all Internet   users an adequate degree of privacy."  Indeed, the IETF has been   doing a significant job in this area {{RFC6973}} {{RFC7258}}, considering  privacy concerns as a subset of security concerns.  {{RFC6973}}

Besides privacy, it should be possible to highlight other aspects of  connectivity embedded in standards and protocols that can have human rights considerations. This report focuses on freedom of expression and the right to association and assembly online. 

Terminology
============

Currently defined in draft-dkg-hrpc-glossary to be folded in at appropriate time.

Link between protocols and human rights
=====================================

+ Include discussion of value laden engineering as discussed in {{Cath}}.  This work discusses four basic architectural principles that are encoded in Internet Technology: 
  ++ Openness, Permissionless Innovation, and Content Agnosticism
  ++ Interoperability
  ++ Redundancy and the Distributed Architecture
  ++ The End-to-End Principle
+ Include discussion of  \"Values and Networks\" work by Roland Bless
+ Include discussion of principles from NetMundial Multistakeholder Statement


Discussion of Universal Declaration of Human Rights (UDHR) and Internet Architecture
--------------------------------------------------------------------

This project is focused on two rights defined in the UDHR {{UDHR}}, Article 19 on Freedom of Expression and Article 20 of Freedom of Association.

Article 19
   :   Everyone has the right to freedom of opinion and expression; this right includes freedom to hold opinions without interference and to seek, receive and impart information and ideas through any media and regardless of frontiers.

Article 20
   :  1 Everyone has the right to freedom of peaceful assembly and association.
   :  2 No one may be compelled to belong to an association.


Theory
--------------

When looking at protocols the considerations can apply from several perspectives.

+   The protocol's direct effects on human rights on the Internet.
-   The protocol's direct effect  on human rights in combination with other protocols
-   The effect of specific protocol elements, separately or in combination with other protocol elements on human rights on the Internet
-   The ability to determine when various effects are occurring, i.e. transparency
-   The effect of deployment or non deployment.  While this may be may seem beyond the protocol itself, often the design of protocol, its difficulty in implementation and the degree to which it contains required elements, poison pills or other protocol artifacts that either encourage or discourse implementation or deployment can be significant in the overall human rights affect of a protocol.


Other relevant research
-------------------------

Look at some of the academic research on the topic including David Post, Jonathan Zittrain and Laura Denardis, among others.

Methodology
============

Currently defined in detail in draft-varon-hrpc-methodolgy to be folded in at appropriate time.  this will largely be a reproduction of Section 3 of that document that focuses on the methodology

Briefly methodology has included:

+ scoping the research problem
- determining terminology to be use linking engineering and human rights concepts
- establishing methodology
- case studies on a set of protocols
- derivation of possible considerations

Case Studies
============

In each of the case studies, the behavior of the protocols is analysed for its positive and negative effects.  In some case these effects are due to the design of the protocol itself, in others they are due to existing or absent features.

Early versions of the analysis on the following protocols are currently being discussed on HRPC list.  Once the discussions have matured those discussions will be folded in this section.

DNS
--------------

Text being done by Will Scott on the HRPC list.

IP
--------------

Text being done by Will Scott on HRPC list.

HTTP
-------------

Text being done by Nex / Claudio on HRPC list.

XMPP
-------------

Text being done by Will Scott on HRPC list.

P2P
-------------

Text being done by Nex on HRPC List.


Possible areas for protocol considerations
==========================================

The case studies point to several areas of protocol behavior that may be appropriate for considerations: 

+ Character encoding for internationalization
- DNS Record
  - Distortion
  - Injection
  - Removal
- Network Poisoning
- Traffic
  - Interception
  - Manipulation
  - Throttling
- User Identification
  - Source and Destination visibility
  - Tracking

Additionally, discussion of the rights themselves and the evidence of these rights being implicits in the IETF design principles {{Clark}} and in some of the existing architecture and protocols, {{Cath}} and {{Liddicoat}} suggest other considerations. {{Cath}} recommends that adhereing to the four fundamental architectural principles discess above is a first step.

Next Steps
============

Once the first take at consideration are defined, what are the next steps for creating something that can be useabble for protocol designers and implementers in considering the human rights of freedom of expression and freedom of association in their work.

Acknowledgement
===============

A section that includes mention the many contributors of text as well as commenters and those who are assisitng this project in existing.

IANA considerations
===================

There shouldn't be any.

Security Considerations
=======================

There shouldn't be any.


