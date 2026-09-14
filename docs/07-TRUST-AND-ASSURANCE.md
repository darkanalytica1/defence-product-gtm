# Trust and assurance as product features

A system that a commander does not trust is a system that will not be used
when it matters, regardless of how accurate it is. This is not a soft point
about user experience. It is the central design constraint for decision
support in this sector.

## Why trust is the binding constraint

An operator carries the consequences of the decision. If your system offers a
recommendation and they cannot tell why, cannot tell how confident it is, and
cannot tell what it would have said with different information, then acting
on it means accepting responsibility for reasoning they cannot inspect.

Faced with that, competent people sensibly fall back on what they can
justify. Your product gets bypassed, quietly, and the feedback you receive is
about the interface.

The pattern generalises: **the willingness to rely on a system is a separate
property from its accuracy, and it has to be designed for deliberately.**

## What earns trust

**Explainability proportional to consequence.** Low stakes output can be
opaque. As consequence rises, the requirement to show reasoning rises with
it. "Here is the answer" is acceptable for a routine filter and unacceptable
for anything that shapes a targeting or safety decision.

**Honest uncertainty.** Systems that express confidence, and whose expressed
confidence turns out to correspond to actual reliability, earn trust quickly.
Systems that present everything with equal assurance destroy it the first
time a confident output is wrong. Being visibly uncertain is a feature.

**Visible provenance.** Where did this come from, how old is it, who else has
it. Under time pressure this is often the first thing an experienced user
looks for, and its absence is disqualifying.

**Graceful degradation.** What the system does when an input is missing, a
feed is stale, or the network partitions. Failing loudly and specifically
("this feed stopped updating eleven minutes ago") builds enormous trust.
Filling the gap silently with the last known value destroys it permanently,
because once a user discovers the system did that, they stop believing
anything it shows.

**Consistency.** The same inputs producing the same output, and behaviour
that does not change unexpectedly between versions. Surprise is expensive
here in a way it is not in consumer software.

## Assurance, which is the formal version

Assurance is the documented, auditable case that a system is safe, secure and
fit for its purpose. Depending on the domain it may cover safety, security
accreditation, airworthiness, or all three, and it is carried out by people
whose job is to be unconvinced.

Three things commercial teams consistently get wrong:

**Treating it as a gate at the end.** Assurance evidence is generated
throughout development or it is reconstructed afterwards at enormous cost.
Retrofitting a safety or security case onto a finished product is one of the
most reliably expensive activities in this industry.

**Underestimating documentation.** The artefacts are part of the deliverable.
A product with excellent engineering and poor documentation is, from the
assurer's position, an unproven product. This is not pedantry. They cannot
certify what they cannot inspect.

**Assuming a change is small.** Whether a change is small is determined by
its assurance impact, not its diff size. A one line change that touches a
safety boundary can be a major event. A large refactor of an isolated
analysis component may be trivial. Architect so that this distinction exists
and is visible, because it will govern how fast you can move for the entire
life of the product. See [08. Roadmapping](08-ROADMAPPING.md).

## Autonomy and automated decision support

Wherever a system recommends or acts rather than merely displays, additional
expectations apply. Broadly, and with wide variation by nation and context:
meaningful human judgement over consequential decisions, clear accountability
that does not evaporate into the software, understandable behaviour, and
predictability under conditions outside the training or design envelope.

Product framing that works: the system is accountable to a person, and its
job is to make that person's judgement better informed and faster, not to
replace it. Product framing that causes problems: the system decides and the
person supervises, which sounds similar and shifts responsibility somewhere
it cannot legitimately rest.

This is a live area of policy and doctrine that differs between countries and
is actively developing. Anything specific in this space needs current,
jurisdiction specific advice.

## The summary for a product manager

Write down, for each output your product produces: what it is based on, how
confident it is, how old it is, what it does when the inputs fail, and who is
accountable for acting on it.

If you can answer those five questions for every output, you have a
defensible product. If you cannot, you have a demonstration.
