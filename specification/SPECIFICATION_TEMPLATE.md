---
title: "Community Specification Template 1.0"
author: "Cem Karan"
date: 2026-08-13T10:57:58-04:00
lastmod: 2026-08-13T10:57:58-04:00
tags:
  - markdown
  - specification
  - template
categories:
  - documentation
description: "A template for writing specifications."
draft: false
---

# Community Specification Template 1.0

Community Specifications are recommended to be drafted in accordance with
international best practices.  Doing so provides clarity, helps adoption, and
also eases the transition of this specification to other standards body if so
desired.  Accordingly, the recommended template below is based on ISO standard
drafting conventions.

To help you, this guide on writing standards was produced by the ISO/TMB and is
available at https://www.iso.org/iso/how-to-write-standards.pdf.

A model manuscript of a draft International Standard (known as “The Rice Model”)
is available at https://www.iso.org/iso/model_document-rice_model.pdf.

In addition, we recommend using the key words "MUST", "MUST NOT", "REQUIRED",
"SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and
"OPTIONAL" as described in [RFC 2119](https://tools.ietf.org/html/rfc2119)

## Title
### Version **Use a https://semver.org 2.0 compatible version number**
### Status **Select one of `Pre-draft`, `Draft`, or `Approved`**

© **Year that this specification was approved**

This specification is subject to the Community Specification License 1.0,
available at [https://github.com/CommunitySpecification/1.0](https://github.com/CommunitySpecification/1.0).

## Contents

- [Foreword](#foreword)
- [Title](#E54C49561CD046F59572559EF805CA51)
- [Scope](#DEE094A1F9844CB89F8694136D40D75B)
- [Normative References](#6153284258224A5F91382A8D18DB4DA2)
- [Terms and Definitions](#E54C49561CD046F59572559EF805CA51)
  - [Term](#8A6373033EFF49AEB746416A64D5EA89)
- [Clause](#67E89A92BD694B27834F248BC1B13515)
  - [Subclause](#839C174CA42F4D5BBD39003964ED3853)
- [Clause](#ECC976252E924621946BD83DF9273259)
  - [Subclause](#41992CA95F504E4C8EE4DCD34D59B04B)
- [Annex A](#0CE5F6985C2D41939D1C785F20E1A08C)
- [Bibliography](#bibliography)

## Foreword

Attention is drawn to the possibility that some of the elements of this document
may be the subject of patent rights. No party shall be held responsible for
identifying any or all such patent rights.

Any trade name used in this document is information given for the convenience of
users and does not constitute an endorsement.

This document was prepared by **Insert name of group**.

This second/third/… edition cancels and replaces the first/second/… edition
(#####:####), which has been technically revised. The main changes compared to
the previous edition are as follows:

**Follow the guidelines at https://keepachangelog.com/en/1.1.0/ when adding
entries here**

—   xxx xxxxxxx xxx xxxx

Known patent licensing exclusions are available in the specification's
repository's `Notices.md` file.

Any feedback or questions on this document should be directed to specifications
repository, located at https://github.com/git-bug/spec.

THESE MATERIALS ARE PROVIDED “AS IS.” The Contributors and Licensees expressly
disclaim any warranties (express, implied, or otherwise), including implied
warranties of merchantability, non-infringement, fitness for a particular
purpose, or title, related to the materials.  The entire risk as to
implementing or otherwise using the materials is assumed by the implementer and
user. IN NO EVENT WILL THE CONTRIBUTORS OR LICENSEES BE LIABLE TO ANY OTHER
PARTY FOR LOST PROFITS OR ANY FORM OF INDIRECT, SPECIAL, INCIDENTAL, OR
CONSEQUENTIAL DAMAGES OF ANY CHARACTER FROM ANY CAUSES OF ACTION OF ANY KIND
WITH RESPECT TO THIS DELIVERABLE OR ITS GOVERNING AGREEMENT, WHETHER BASED ON
BREACH OF CONTRACT, TORT (INCLUDING NEGLIGENCE), OR OTHERWISE, AND WHETHER OR
NOT THE OTHER MEMBER HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

<a id="E54C49561CD046F59572559EF805CA51"></a>
## Title (Introductory element — Main element — Part : Part title) **This section is mandatory**

**Introductory text goes here**

<a id="DEE094A1F9844CB89F8694136D40D75B"></a>
### Scope **This section is mandatory**

**Text regarding the scope of this specification goes here.  This section is
free-form, but a reader SHOULD be able to determine both what the specification
covers, and what it doesn't cover.**

<a id="6153284258224A5F91382A8D18DB4DA2"></a>
### Normative References **This section is mandatory**

**There are two options of text you may use here (shown below).  Select the
  block quote of the appropriate option, and replace all text in this section
  with the contents of that block quote.**

- The normative references shall be introduced by the following wording:

  > The following documents are referred to in the text in such a way that some
  > or all of their content constitutes requirements of this document. For dated
  > references, only the edition cited applies. For undated references, the
  > latest edition of the referenced document (including any amendments)
  > applies.
  >
  > ISO ##### #, General title — Part #: Title of part
  >
  > ISO ##### ##:20##, General title — Part ##: Title of part

- If no references exist, include the following phrase below the clause title:

  > There are no normative references in this document.

<a id="E54C49561CD046F59572559EF805CA51"></a>
### Terms and Definitions **This section is mandatory**

**There are four options of text you may use here (shown below).  Select the
  block quote of the appropriate option, and replace all text in this section
  with the contents of that block quote.**

- If all the specific terms and definitions are provided in this section of this
  document, use the following introductory text:

  > For the purposes of this document, the following terms and definitions
  > apply.

- If this document refers an external document (or documents), use the following
  introductory text:

  > For the purposes of this document, the terms and definitions given in the
  > following apply:

  and provide a list of referenced documents.  Note that documents you refer to
  in this section are considered to be *normative*; that is to say, to
  correctly implement the specification within this document, an implementation
  MUST *also* correctly implement *all* specifications listed within this
  section.

- If terms and definitions are provided in this section in addition to a
  reference to an external document, use the following introductory text:

  > For the purposes of this document, the terms and definitions defined in this
  > section and given in the following apply:

- If there are no terms and definitions provided, use the following introductory
  text:

  > No terms and definitions are listed in this document.

The text below is always included after each option:

> ISO and IEC maintain terminological databases for use in standardization at
> the following addresses:
>
> —   ISO Online browsing platform: available at https://www.iso.org/obp
> —   IEC Electropedia: available at http://www.electropedia.org/

**WHEN WRITING SPECIFICATIONS, ENSURE THAT THERE ARE NO CONFLICTS BETWEEN ANY OF
  THE DEFINITIONS IN ANY OF THE DOCUMENTS!  There are several methods to ensure
  that this is true; here are two:**

- State that conflicts are defects within this specification, and request
  readers file a bug report.  This is generally the most appropriate method.
- Define a total ordering over all documents recursively (i.e., created an
  ordered list of documents).  The last definition of a term is the prevailing
  one.  While this method works, it can sometimes lead to surprising results
  and is often difficult to achieve in practice.  Where possible, avoid doing
  this.

<a id="8A6373033EFF49AEB746416A64D5EA89"></a>
#### Title **Each term or definition MUST have its own section**

**Text defining the term.  This text is mandatory.  The section itself is
  free-form, and MAY contain notes, diagrams, or references to other previously
  defined terms or clauses as needed to completely and without ambiguity define
  this term.  You MAY direct readers to as-yet undefined terms or clauses as
  additional areas of interest so long as knowledge of the undefined isn't
  required to define this term.  Where it makes the exposition clearer to do
  so, feel free to add in subsections within a term's section. As a note, terms
  and definitions usually correlate to data types in programming languages;
  they are what the specification operates on.**

<a id="67E89A92BD694B27834F248BC1B13515"></a>
### Clause **Each clause MUST have its own section**

**Text defining the clause.  This text is mandatory.  The section itself is
  free-form, and MAY contain notes, diagrams, or references to other previously
  defined terms or clauses as needed to completely and without ambiguity define
  this clause.  You MAY direct readers to as-yet undefined terms or clauses as
  additional areas of interest so long as knowledge of the undefined isn't
  required to define this clause.  Where it makes the exposition clearer to do
  so, feel free to add in subsections within a clause's section. As a note,
  clauses usually correlate to functions in programming languages; they operate
  on the terms and definitions previously defined to produce an effect or
  output.**

<a id="839C174CA42F4D5BBD39003964ED3853"></a>
#### Subclause **optional**

**An optional subclause**

<a id="ECC976252E924621946BD83DF9273259"></a>
### A Different Clause

**A different clause.  This clause MAY use any term or clause previously
  defined (including in normative references) in its own definition.**

<a id="41992CA95F504E4C8EE4DCD34D59B04B"></a>
#### Subclause **optional**

**An optional subclause**

<a id="0CE5F6985C2D41939D1C785F20E1A08C"></a>
## Annex A **Make sure that the title is clear and informative**

**The first line of text within an annex must be either `(informative)` or
  `(normative)`.  The text must be on a line by itself, as shown below**

(informative)

In general, annexes are informative, not normative.  They may contain examples,
text vectors, or possibly, alternative forms of the definitions in the main
text of the document.  A particularly good example of this is when a
programming language collects the syntax into a single formal grammar in an
annex; by itself, the grammar is likely to be difficult to understand, but its
formality may make it easier to create a parser.

In some cases, you may choose to use a normative annex so as to avoid breaking
up the flow of the main body of text.  A good example of this would be a set of
CAD drawings, or other lengthy normative data.  In such cases, it's best to
both put that data into an annex and to supply the data in an appropriate data
format as a separate archive file that a computer can easily parse.  What you
choose to do is up to you, but regardless of what you choose, normative
materials MUST be accessible along with the specification itself.  Typical
examples of this are specifications that are bundled into TAR or ZIP archives
along with the normative data.  This ensures that implementers have access to
all material that they require to implement the specification correctly.

## Bibliography

[1] ISO ##### #, General title — Part #: Title of part

[2] ISO ##### ##:20##, General title — Part ##: Title of part
