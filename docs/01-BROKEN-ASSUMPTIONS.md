# Why defence breaks commercial product assumptions

Seven assumptions, and what replaces each. If you internalise this document
the rest of the guide is detail.

## 1. "I can talk to my users"

**Commercial:** you book thirty customer interviews and watch session
recordings.

**Defence:** your users may be unreachable by policy, not by inconvenience.
They may be deployed, they may be prohibited from discussing what they do,
and the interesting parts of their workflow may be classified at a level you
do not hold. The people who will talk to you freely are often the people
furthest from the actual work.

**What replaces it:** structured proxies. Former operators now in industry,
training establishments, exercises and wargames, doctrine and published
lessons learned, and the requirement documents themselves, which are a
distillation of user need written by someone whose job was to capture it.
None of these is as good as watching a user work. All of them together are
better than guessing. See [11. Discovery](11-DISCOVERY.md).

## 2. "The person with the pain has the budget"

**Commercial:** the head of sales feels the pain, the head of sales has a
card, the deal closes.

**Defence:** the person with the pain is a serving operator with no budget
authority whatsoever. The budget sits with a programme office that answers to
a capability plan written years earlier. Pain does not convert into purchase
without travelling through a requirements process.

**What replaces it:** understanding that your champion's job is not to buy
your product. It is to make the case internally, in the language of
capability, against a documented gap. Your job is to arm them for that
argument. See [02. The buyer map](02-THE-BUYER-MAP.md).

## 3. "A pilot leads to a rollout"

**Commercial:** land and expand. Get one team using it, let it spread.

**Defence:** pilots, trials and experiments are a recognised and well funded
activity, and they very often lead nowhere, not because the technology
failed, but because no route existed from experiment to programme of record.
Money for trying things and money for buying things come from different
places and follow different rules.

**What replaces it:** ask, before the trial starts, what the transition path
is. Who would own this in service, which budget line would fund it, what
would have to be true for it to be adopted. If nobody can answer, you are
being used to explore an idea, which is a legitimate thing to be paid for,
but it is not a sales pipeline. Treat it as research revenue and plan
accordingly.

## 4. "We ship weekly"

**Commercial:** continuous deployment is a virtue and a differentiator.

**Defence:** a change to a system that has been accredited for operational
use may invalidate that accreditation. Changing software on a platform can
require retesting, recertification, redocumentation and retraining. The
sector is actively working on making this faster, and in some domains it now
genuinely is, but the constraint is real and it is there for a reason.

**What replaces it:** architecture that separates what can change quickly
from what cannot. The parts of your system that touch safety, security
boundaries or platform integration change slowly and deliberately. The parts
that are analysis, presentation and workflow can often change much faster.
Product teams that win here design that seam early. Teams that do not find
that their entire product inherits the slowest release cadence of its most
constrained component.

## 5. "Our roadmap is ours"

**Commercial:** you decide what to build, informed by customers.

**Defence:** a substantial part of your roadmap will be contractually
specified, because the customer bought a capability against a requirement and
the requirement says what it must do. Meanwhile the parts nobody specified,
interoperability with systems you have never heard of, may be the parts that
decide whether you are adopted.

**What replaces it:** a roadmap in two layers. The contracted layer, which is
committed and dated, and the capability layer, where you invest ahead of
requirements because you believe where the need is going. Confusing the two
is how product teams end up delivering everything they promised and still
losing the follow on competition.

## 6. "Pricing scales with usage"

**Commercial:** seats, consumption, tiers.

**Defence:** the customer may need to know the total cost of ownership over
twenty years before they can approve anything, and a model where the price
rises with success can be difficult to fund, because the budget was set in
advance and does not respond to your product being popular.

**What replaces it:** predictability. Models built around delivery,
integration, support and enhancement rather than headcount. See
[10. Commercial models](10-COMMERCIAL-MODELS.md).

## 7. "Fast is better"

**Commercial:** unambiguously true.

**Defence:** true, but measured differently. The sector talks about getting
capability to the people who need it at the speed the situation demands. That
clock starts when the need appears, not when your sprint starts, and it stops
when the capability is usable in the field, not when you merge the pull
request. Qualification, accreditation, training, documentation and support
arrangements are all inside the clock.

**What replaces it:** optimising the whole path rather than your own segment
of it. A product that is designed to be easy to accredit, easy to train on,
and easy to support is genuinely faster in the only sense the customer
measures, even if the engineering team ships less often.

## The pattern behind all seven

Commercial product management optimises for **learning speed**, because in a
competitive market the firm that understands the customer first wins.

Defence acquisition optimises for **accountability and integration**, because
the buyer is spending public money on something that must work with other
people's equipment, in conditions nobody can fully rehearse, with
consequences that are not commercial.

Neither is wrong. They are answers to different questions. Most of the
friction a commercial team feels entering defence comes from applying the
first optimisation to the second problem and concluding the customer is
broken.
