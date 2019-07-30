# Administrivia

This repository tracks PING's meta-work.

2019 charter draft: https://w3cping.github.io/administrivia/charter-draft.html

# PING Process

PING's goal is to ensure that the specifications recommended by the W3C respect the privacy of people who use the web platform, and ensure that the web platform is an environment which allows people to browse the web privately.

PING's core administrative mechanism for achieving this is _horizontal review_: members of PING review specifications and provide recommendations to the authors about how to ensure that their specifications support a web platform which respects privacy. This formal review process is the most visible part of a larger iceberg of activities aimed at helping specification authors write with privacy in mind. The best place to make privacy-related improvements to specifications is substantially in advance of horizontal review points. PING welcomes conversations with authors at all phases of specification development. Ideally, PING would be thoroughly familiar with specifications, their potential privacy impacts, and the measures takes to mitigate those impacts well before the time horizontal review points are reached, and those privacy reviews would consist mostly of codifying & recording conversations which have already happened, rather than pointing new things out to authors.

PING's work extends substantially beyond the specific task of ensuring that a high privacy standard is upheld in those specifications which become recommendations. We also work with other privacy focused groups and researchers to gain better understanding of privacy risks and solutions for the web, ensure W3C processes protect privacy as a first-class feature of the Web. The remainder of this document focuses exclusively on the procedure of privacy reviews.

## Privacy Review

Every specification seeking recommendation status must be reviewed by PING. Specification authors request review by opening an issue in the [`w3cping/privacy-reviews`](https://github.com/w3cping) GitHub repository, using the supplied privacy review issue template. This issue should include as much context as possible so that PING can understand the aims and working environment of the specification.

**A review will either result in PING raising issues, raising serious concerns, or raising neither.**

Review is not a sign-off or authorization step — it involves substantial engagement with the design and implementation of the specification as well as its goals and likely impact on the web platform. PING recommends that specification authors ask PING to start a review as soon as they have the broad outline of a specification, and no less than once every six months during a specification's lifespan. Many privacy issues can be anticipated at this early stage. Learning about these potential issues allows working groups and specification authors to implement solutions smoothly and thoughtfully. This should lead to fewer issues raised during review.

### Raising Issues

**Issues** are specific privacy drawbacks with the specification which must be addressed before the specification becomes a recommendation. When raising issues, PING will endeavor to articulate posssible technical approaches which mitigate those issues.

When issue are raised, PING will open GitHub issues in the specification's repository describing the concern and potential options for solutions. If the specification's working group do not use GitHub issues, they should specify an alternative issue tracking location in the review request, and PING will use that instead. PING will also list each issue opened in the privacy review request.

Specification authors should work with PING to resolve these issues. Once all issues have been resolved to the satisfaction of the authors and of PING, PING will resolve the privacy review request.

### Serious Concerns

**Serious Concerns** are fundamental problems with the approach or goals of the specification. These are unlikely to have straightforward technical remediations. They require fundamentally re-thinking or re-architecting the specification. This should be rare.

When there are serious concerns with a specification, PING will outline them in a response to the privacy review request. Specification authors should work with PING to understand these concerns and re-architect the specification, which may require re-chartering. When the specification has been re-thought in this way, specification authors should open a new privacy review request for the new specification

## Review Status

Every specification is therefore in one of four possible states:

1. This specification has been reviewed by PING. There are no issues or concerns.
2. This specification has been reviewed by PING. There are issues to resolve.
3. This specification has been reviewed by PING. PING has serious concerns! [There may also be issues to resolve.]
4. This specification has not been reviewed by PING.

This status should be indicated at the top of all specification documents, alongside the similar status from other horizontal review groups.

Specifications which are not in state #1 are not eligible to proceed to recommendation status.

In addition, implementers should avoid working from specifications in state #2 or (especially) in state #3 since these specifications require substantive changes, and because implementing these specifications may harm the privacy of those who use the web platform.
