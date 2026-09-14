# Interoperability is a requirement, not an integration

In commercial software, integrations are something you add once a customer
asks. There is a page on your website listing them, and adding one is a
quarter's work for a small team.

In defence, the ability to work with other people's systems is frequently the
primary requirement, and everything your product does on its own is
secondary. A capability that cannot exchange information with the systems
around it is not a partial success. It is often simply not adoptable.

## Why it is structural

The customer is rarely buying a system. They are adding a component to a
system of systems that already exists, that was bought over decades, and that
includes equipment belonging to other nations who will not modify anything
for your convenience.

Multiply that by coalition operations, where the participants are decided by
politics shortly before the event, and the requirement becomes clear: work
with things you have not seen, operated by people you have not met, on a
network assembled last week.

## The three levels

It helps to separate interoperability into levels, because products often
achieve one and claim all three.

**Technical.** Can the bits move. Networks, protocols, transports,
encryption. Necessary, and the easiest of the three.

**Syntactic.** Can the receiving system parse it. Shared formats, message
standards, schemas. Harder, and where most standards work sits.

**Semantic.** Does the receiving system understand the same thing by it. This
is where interoperability actually fails. Two systems can exchange a
perfectly valid message about a "track" and mean materially different things
by the confidence attached to it, the time it refers to, or what counts as
the same object seen twice.

Semantic failures are dangerous precisely because they are silent. Nothing
errors. The picture just becomes subtly wrong, and the people using it have
no indication.

If you take one design principle from this document: **carry meaning
explicitly**. Units, time reference, confidence, source, and what the
identifier refers to. Assume the receiver's assumptions differ from yours,
because they do.

## Standards, and how to think about them

Alliances and national authorities publish agreed standards covering message
formats, data models, symbology, interfaces and procedures. There are a great
many, they overlap, they have versions, and different participants implement
different subsets.

Practical guidance:

- **Find out which standards the specific customer actually uses**, at which
  version, and with which local variations. The general answer is much less
  useful than the specific one, and there is almost always local variation.
- **Conformance is claimed more often than achieved.** "Supports standard X"
  can mean anything from full conformance to reading one message type. Ask
  what has been tested, against what, and by whom.
- **Test events matter.** Periodic interoperability exercises where suppliers
  connect their equipment and find out what actually works are the real
  currency of credibility here. Participating is expensive and it is worth it,
  because "we tested this against nine other systems at a recognised event"
  is evidence, and a conformance claim in a brochure is not.
- **Standards lag reality.** New capability arrives before the standard that
  describes it. Being early is an advantage only if you stay compatible when
  the standard lands, so isolate your own extensions behind a boundary you
  can change.

## Federation rather than unification

A recurring theme in modern thinking is that you will not get one network,
one system or one data model. You get a temporary federation of many, formed
for a particular operation, with participants joining and leaving.

Design implications follow directly:

- Assume you are a guest on someone else's network, not the host.
- Assume you will be asked to join a federation at short notice, and that
  the onboarding effort will be judged.
- Assume participants will have different permissions over the same data.
- Assume the federation will partition, and that both sides must keep working
  and reconcile later.

That last one is worth dwelling on. Partition tolerance is a normal
engineering topic in distributed systems, and here it is an operational
requirement, because the network will be attacked or simply fail. A product
that requires continuous connectivity to a central service is making a strong
assumption about an environment designed to violate it.

## The commercial consequence

Interoperability work is unglamorous, hard to demonstrate, and rarely what
gets a product noticed.

It is also, repeatedly, what decides procurements. Budget for it as a
first class part of the product, staff it with people who enjoy it, and
describe it precisely and honestly in your proposals. Precision here is
itself a differentiator, because vagueness about interoperability is so
common that specificity reads as competence.
