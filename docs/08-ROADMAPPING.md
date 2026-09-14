# Roadmapping against programme cycles

Your planning horizon is a quarter. Your customer's is a decade. This
document is about living with that.

## The mismatch

A commercial roadmap assumes you can change direction when you learn
something. A defence programme assumes commitments made years ago will be
honoured, because other commitments were made on the strength of them.

Both are rational. The friction is structural and permanent, and the job is
to manage it rather than resolve it.

## The two layer roadmap

The only structure I have seen work consistently separates the roadmap into
two layers with different rules.

**The committed layer.** What you have contracted to deliver, with dates,
acceptance criteria and consequences. This is close to a construction
schedule. It changes through a formal process, it is communicated
carefully, and the discipline is absolute. Missing a date here is not a
missed sprint goal, it is a contractual event that may cascade into other
people's programmes.

**The capability layer.** What you are building because you believe the need
is coming, ahead of anyone specifying it. This is funded by you, it moves
when you learn, and it is where your actual product strategy lives.

The committed layer keeps you in business. The capability layer decides
whether you win the next competition. Teams that only have the first become
contractors who build what they are told and are competed away on price.
Teams that only have the second build impressive things nobody buys.

## Architecting for two speeds

Because assurance impact rather than code size determines how fast a change
can ship, the highest leverage architectural decision you make is where to
put the boundaries.

Aim for a separation roughly along these lines:

| Layer | Changes | Why |
| --- | --- | --- |
| Platform integration, safety and security boundaries | Slowly, deliberately | Every change carries assurance cost |
| Core processing and data handling | Moderately | Testable, but consequential |
| Analysis, workflow, presentation, reporting | Quickly | Contained blast radius |

Get this wrong and your whole product inherits the release cadence of its
most constrained part, which is the single most common cause of a defence
software team feeling permanently slow.

Get it right and you can honestly tell a customer that certain categories of
enhancement are quick, which is unusual enough in this market to be a
selling point.

## Planning around the money

Budgets are annual and set in advance, and they distinguish sharply between
money for investigating things and money for buying things. Practical
consequences:

- **Know which budget your opportunity sits in.** Research money and
  procurement money behave completely differently and rarely convert into one
  another without a deliberate transition plan.
- **The cycle has a shape.** There are periods when new commitments can be
  made and periods when they cannot. Learn your customer's rhythm; it is not
  a secret, and aligning your proposals to it materially improves your hit
  rate.
- **Support and enhancement is where the durable revenue is.** The initial
  delivery is often the smaller half of the whole life value. Design the
  commercial arrangement, and the product, on that basis. See
  [10. Commercial models](10-COMMERCIAL-MODELS.md).

## Communicating a roadmap externally

Three rules that have served well:

**Never show a date you are not willing to be held to.** In commercial
software an aspirational roadmap slide is understood as aspiration. Here it
may be read as a commitment and repeated in someone else's planning document.

**Distinguish committed from intended, explicitly and visibly.** Customers
respect the distinction and are used to it. What damages credibility is
presenting the second as the first and then moving it.

**Update when things change, before you are asked.** The reputational cost of
a slip you disclosed early is a fraction of the cost of one discovered late.
This sector has a long memory and a small population.
