# Command and control for product people

Command and control, universally shortened to C2, is the single most useful
concept for a product person in this sector, because almost every defence
software product is somewhere inside it, whether or not the team building it
uses the term.

## What it actually means

Strip away the jargon and C2 is the answer to two questions:

- **Who decides what**, and on what authority.
- **How does what they decided become action**, and how do they find out
  whether it worked.

That is it. Command is the authority to decide and the responsibility for the
consequences. Control is the machinery by which decisions turn into activity
and information about that activity returns.

It is worth noticing how ordinary this is. Every organisation has C2. A
hospital has it, an airline has it, your company has it. The military
difference is that the stakes are higher, the environment is actively hostile
to the machinery, and the consequences of ambiguity are severe, so the subject
has been studied formally for a very long time.

## The loop, and why everyone talks about it

The recurring mental model is a cycle: observe what is happening, make sense
of it, decide, act, then observe the result. Different communities name the
steps differently and argue about the details. The important properties are:

- **It is a loop, not a pipeline.** Output feeds back into input.
- **It has a period.** How long one turn takes.
- **It degrades.** Under stress, under attack, and when information is
  missing or wrong, the loop slows down or produces worse decisions.

Almost every defence software product on the market claims to improve this
loop. Being specific about *which part* you improve, and being honest about
the parts you do not, is an unusually effective differentiator, because most
marketing in this space claims all of it.

## Where products sit in the loop

| Part of the loop | What products here do | Typical failure mode |
| --- | --- | --- |
| Observe | Sensors, collection, feeds, ingestion | Volume without relevance |
| Make sense | Fusion, correlation, analysis, visualisation | Confident output from weak input |
| Decide | Options, planning, wargaming, decision support | Recommending without explaining |
| Act | Tasking, orders, dissemination, execution monitoring | Assuming the order arrived and was understood |
| Learn | Assessment, after action review | Measuring activity rather than effect |

Ask yourself which row you are in. Then ask which row your customer thinks
you are in. Products fail in this market when those two answers differ,
because the customer bought a decision aid and received a data display.

## The three dimensions that matter commercially

A useful way to think about where C2 problems actually live, and one that
maps well onto what product teams can influence:

**Process and structure.** Who reports to whom, what a headquarters is
organised to do, how authority is delegated. Largely outside your control,
entirely determinative of whether your product fits. A tool that assumes a
flatter or faster authority structure than the organisation has will be
rejected for reasons that look like usability complaints.

**Information and knowledge.** What is collected, how it is described, who
may see it, how it is shared, and how it retains meaning as it moves. This is
where most software products actually live, and where interoperability and
data standards bite. See [06. Interoperability](06-INTEROPERABILITY.md).

**Human factors.** Cognitive load, training burden, fatigue, trust,
situational awareness, and what happens when the person using your product
has been awake for twenty hours. This is the dimension commercial teams most
underestimate and the one that most often determines adoption. See
[07. Trust and assurance](07-TRUST-AND-ASSURANCE.md).

## Two terms you will hear

**Speed of relevance.** Being fast enough to matter, which is a relative
standard rather than an absolute one. A decision that would have been correct
an hour ago may be worthless now. This reframes speed usefully: the question
is never "how fast is your system" but "is the whole chain fast enough given
what the other side is doing". It also means that a very fast component
inside a slow chain has added nothing, which is a hard message for a product
team that has optimised the wrong segment.

**Mission command.** A philosophy of telling subordinates what outcome you
want and why, then leaving them to work out how. It requires trust in both
directions and shared understanding of intent. Its relevance to product
design is direct and often missed: a system that requires central approval
for every action, or that gives a commander perfect visibility of everything
a subordinate is doing, can quietly undermine the doctrine the organisation
actually runs on. Technical capability and command philosophy can conflict,
and when they do, the philosophy usually wins.

## Why this matters for what you build

If C2 is about who decides and how decisions become action, then your product
is not really a data product, an analytics product or a visualisation
product. It is an intervention in somebody's decision making under pressure,
accountability and uncertainty.

Products designed with that framing tend to be explainable, to degrade
gracefully, to respect the authority structure they sit inside, and to be
honest about their own uncertainty.

Products designed without it tend to be beautiful, impressive in
demonstrations, and quietly unused.
