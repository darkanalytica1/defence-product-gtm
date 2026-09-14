# Dual use go to market

You have a commercial product that works. Defence looks like a large adjacent
market with real budgets. This document is about what actually happens next.

## First, decide whether you mean it

Defence is not an adjacent market you can address opportunistically with your
existing team. It is a different business with its own compliance,
contracting, security and support obligations, and entering it changes your
company.

Honest questions before committing:

- Are you prepared for sales cycles measured in years, with costs incurred
  long before revenue?
- Can you carry the compliance burden: quality accreditation, security
  requirements, export control, personnel clearance where needed?
- Will your commercial customers be comfortable with your defence work, and
  your defence customers with your commercial work? Usually yes, occasionally
  not, and it is better to know early.
- Can your investors and board tolerate the cash flow shape and the
  disclosure limits?
- Are you willing to support a version of your product for many years,
  potentially long after the commercial version has moved on?

A "no" to any of these is not disqualifying, but it needs a plan rather than
optimism.

## The realistic entry routes

**Through a prime or systems integrator.** Most small suppliers never
contract directly with a ministry. They supply a larger company that holds
the integration responsibility and the customer relationship. Faster to
start, lower compliance burden initially, and you give up margin and direct
customer access. This is the default route and there is no shame in it.

**Through research and innovation funding.** Most countries and the alliance
level bodies run programmes designed to bring newer suppliers in. Genuinely
useful for building credibility, understanding the customer and de-risking
technology. The trap is described in
[01. Broken assumptions](01-BROKEN-ASSUMPTIONS.md): a trial is not a sale, and
some organisations subsist indefinitely on trial funding while never
transitioning to a programme. Ask about the transition path at the start.

**Through an adjacent public customer.** Border agencies, coastguards,
emergency services, critical infrastructure operators and civil aviation
often have related needs, lower barriers, and procurement processes closer to
normal public sector buying. A credible reference from one of these is
meaningful in defence, and the route is systematically underused.

**Directly, via open competition.** Realistic mainly for well defined
commodity supply or where you are unusually well positioned. Expensive to
pursue cold.

## The traps

**Assuming your commercial product is the product.** It is the starting
point. What gets bought usually differs in deployment model, connectivity
assumptions, data handling, logging, accreditation evidence, and support
commitments. Budget for that gap honestly. It is typically larger than the
first estimate.

**Building a defence fork you cannot maintain.** Two codebases diverging
slowly is one of the most reliable ways to destroy a small company's
engineering velocity. Configuration over forking, wherever it can possibly be
made to work.

**Underestimating the support obligation.** A twenty year support commitment
is a real liability that has to be priced, staffed and planned, and it will
outlast your current architecture, your current dependencies and probably
several of your current engineers.

**Taking the first contract on any terms.** Terms set precedent. Intellectual
property, liability, support obligations and data rights conceded in a small
first contract have a way of becoming the baseline for every subsequent one.
Get advice before signing, not after.

**Hiring only from defence, or only from commercial.** Teams drawn entirely
from one side reliably fail in a predictable direction: pure defence
backgrounds build slowly and conservatively, pure commercial backgrounds
build things that cannot be accredited. The useful team is mixed and spends
its first year translating between two vocabularies.

## What genuinely transfers from commercial

It is worth being clear that the commercial background is an asset, not just
a handicap to be corrected.

User centred design is rare and valued. Modern engineering practice,
automated testing, observability and deployment discipline are genuinely
ahead of much of the sector. Speed of iteration, applied where assurance
permits, is a real advantage. And an outside perspective on a problem that
has been looked at the same way for thirty years is occasionally worth a
great deal.

The winning position is not "we are a commercial company selling to defence"
and not "we have become a defence contractor". It is a company that has
learned the constraints well enough to take them seriously, and kept enough
of its original engineering culture to be worth hiring in the first place.
