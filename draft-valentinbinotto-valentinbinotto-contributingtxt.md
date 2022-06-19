---
title: "contributing.txt -  a simple way to provide informations for contributors"
abbrev: "contributing.txt"
category: info

docname: draft-valentinbinotto-valentinbinotto-contributingtxt-latest
submissiontype: IETF  # also: "independent", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
area: AREA
workgroup: WG Working Group
keyword:
 - next generation
 - unicorn
 - sparkling distributed ledger
venue:
  group: V434 Project
  type: Working Group
  mail: rfc@vauly.net
  arch: https://v434.info/id-valentin-contributingtxt/draft-valentinbinotto-valentinbinotto-contributingtxt.txt
  github: valentinbinotto/id-valentin-contributingtxt
  latest: https://v434.info/id-valentin-contributingtxt/draft-valentinbinotto-valentinbinotto-contributingtxt.txt

author:
 -
    fullname: Valentin Binotto
    organization: valentinbinotto
    email: "valentinbinotto@v434.net"

normative:

informative:


--- abstract

Open source projects rely on the cooperation of third parties.  Other websites also rely on user feedback, for example, when bugs occur. There are various platforms that enable effective collaboration. However, this diversity also presents a challenge. Where should users who have discovered an error report it? Or how can third parties participate in a project? This document presents one way to communicate such information in a consistent manner.

--- middle

# Introduction
Currently, there are various platforms for collaboration on projects or communication with users of websites, services and so on. This creates opportunities, for example in open source projects, to work with contributors and exchange information. However, such opportunities differ from project to project. Users who are interested in participating in a project need to be aware of these different procedures. This can be a challenge due to the inconsistent form of the information and might also lead to users deciding not to participate because they cannot find a contact point. <br><br>At the same time, there is a need for "bug reports" in other forms of websites as well. Users are expected to point out bugs to the person in charge and thus lead to a better user experience for all users. Unfortunately, the ways and procedures for such "bug reports" also differ from website to website. These differences mean that users might not be able to find a contact person to report a bug, and thus fail to report it.

The goal of this document and the proposed form of communication in the "contributing.txt" file is:

1. to provide open source or similar projects with the opportunity to inform interested parties about the possibilities of contributing.
2. to offer any kind of website the possibility to define a contact person for bug reports etc.



# Conventions and Definitions

{::boilerplate bcp14-tagged}


# The Specification
This document defines a file called "contributing.txt", which provides information about possible contribution to a project or website.  The file format of "contributing.txt" MUST be plain text (MIME type "text/plain") (Section 4.1.3 of RFC2046) and MUST be encoded using UTF-8 (RFC3629).<br><br>The file "contributing.txt" MUST be placed in the ".well-known" directory (for example: example.com/.well-known/contributing.txt). Additionally, a copy can optionally be stored directly under the domain (for example: example.com/contributing.txt).<br><br>The file "contributing.txt" MUST contain at least:

1. Paragraph "Admin" with the name of the administrator or the webmaster
2. Paragraph "Bugs" with a mail address or a web address to report bugs

Example:

Admin: Valentin Binotto
Bugs: bugs@vauly.net


OPTIONALLY the following paragraphs can be added to the "contributing.txt" file:

3. Paragraph "Open Source" with a web address to a suitable platform for third party collaboration (for example github.com or gitlab.com)
4. Paragraph "License" with information about the license that applies to the content of the website.
5. Paragraph "Guidelines" with a web address to the guidelines for contributing to this project.

Example:

Open Source: github.com/valentinbinotto
License: Creative Commons Attribution 4.0 International Public License
Guidelines: github.com/valentinbinotto/v434/guidelines.txt


OPTIONALLY, comments can be added to the "contributing.txt" file. Each line of the comment must start with "#" (%x23).

Example: 

Hello, world!


The specified paragraphs must be placed in the specified order. Only one entry is allowed per paragraph



However, paragraphs can be reused an unlimited number of times, as long as the order of the paragraphs is still as specified.

Example for a "hdhdszu.txt" file:



Admin: Valentin Binotto
Bugs: bugs@vauly.net
Open Source: github.com/valentinbino
License: Creative Commons Attribution 4.0 International Public License
Guidelines: github.com/valentinbinotto/v434/guidelines.txt
Valentin Binotto
92ee219838c69464862e86cb67549d1ab1eae3a7fa0d8925970fea303a72849e


# Security Considerations

Because of the use of URIs and well-known resources, security considerations of [RFC3986] and [RFC8615] apply here.

# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.