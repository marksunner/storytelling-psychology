# Where Are the Receipts?

*A small piece of mental equipment for telling the real thing from the chaff. Companion to [The Story Doesn't Care If It's True](01-the-story-doesnt-care.md).*

---

You are leaving the supermarket with a week's shopping when the alarm at the door goes off. Heads turn. The security guard, who deals with real shoplifters every week, starts towards you, and his expression is not friendly. Shoppers wheeling past give you the particular look people reserve for someone who has just been caught. Nothing about you has changed in the last five seconds. You are exactly the person who queued, paid and said thank you at the till; somewhere in your bags is an item with a security tag the checkout missed. But an alarm is loud, confident and wrong, and everyone in earshot has already reached a conclusion.

Now notice what you reach for. Not your sincerity. You do not try to look honest, because you know, without ever having thought about it, that an honest face and a guilty one are indistinguishable from the outside. You reach for the receipt. One small piece of paper outvotes the alarm, the guard's suspicion and the certainty of every stranger watching, because it is the only thing in that doorway that does not depend on being believed. It can simply be checked. Sincerity and truth are two different things that often travel together and sometimes do not, and in that moment you know exactly which of the two gets you out of the building.

You carry this instinct everywhere, on both sides of the counter. When a mechanic says the gearbox is gone, you want to see the old one, or you get a second opinion. When a builder's final bill is double the quote, you ask for it itemised. When a headline about your own street sounds off, you walk down and look. In the ordinary business of your life you are a competent, instinctive auditor, and you would be insulted to be told otherwise.

And then you open the news, or a feed, and the auditor goes to sleep. The part of you that would never try to walk past that guard on charm alone will accept "studies show," "experts agree," and "everyone knows" without asking to see anything at all. And the sleep is not random. Your scrutiny fades most reliably at the precise moment a claim arrives already agreeing with you. When something confirms what you hoped was true, or flatters the side you already stand on, or completes a story you were enjoying, the demand for a receipt feels almost rude, like doubting a friend. So you wave it through. Truth and a satisfying story feel identical from the inside. Only the receipt can tell them apart.

I could leave that as an assertion, the way essays like this usually do. Instead, let me show you the moment I found out it was true of me.

## The author fails his own test

This July I spent three days hunting a fault in a machine I keep in my study: four small computers wired together to run a large AI model locally. The fault was maddening. At unpredictable moments, sometimes mid-sentence, the whole system would silently freeze, and nothing in the ordinary diagnostics said why.

The hunt was carried out jointly with an AI assistant, and that arrangement forced a house rule on us from the first hour. An AI is the most fluent, most confident explainer you will ever meet, and its explanations cost nothing to produce. It can hand you three beautiful theories of your bug before your coffee has cooled, each internally consistent, each wrong in a different way. So the rule was blunt: narrative is never evidence. A claim counted only when it arrived pinned to a receipt. A log line. A process listing. A configuration value read back from the live system. However plausible the story, however confidently told, and by whomever: no receipt, no belief.

I thought of this as a rule for auditing the machine. On the second day it audited me.

I stated, from memory and with complete confidence, that a particular limit in the system was set to 128K. I was not guessing. I remembered setting it. I could picture myself doing it. Then we read the actual configuration back from the running system, and the receipt said 120K. My sincerity was perfect. My memory was specific and vivid. And it was wrong, and nobody had deceived me except me. I had been walking around with a small false fact filed under "true," and it felt exactly like all my other facts, and if the house rule had not applied to me as well as to the machine, it would be there still.

Two things came out of those three days. The first was the fault itself: the trail of receipts led, step by step, past every plausible story, to a genuine defect buried deep in a vendor's software, which we documented and published. The second was this essay. And since it would be absurd to write about receipts without producing one, the evidence from that hunt is [public](https://github.com/marksunner/glm52-dgx-spark-deadlock-evidence), every log, test and correction, including the place where my 128K died. You can check it. That is rather the point.

## What still costs something

The companion essay ends on a warning: fluent, confident, well shaped narrative is now generated at scale, essentially for free, and pointed at you through every screen you own. This essay answers the question that warning leaves hanging. If fluency is free, what still costs something?

A receipt does. A receipt is the part of a claim that exists outside the teller. The bank record, the log line, the ruling, the dataset, the primary document: the thing that stays the same size no matter how the story around it grows. Producing one requires the event to have actually happened, which is precisely the cost a fabricator cannot pay. That is why the receipt, and not confidence, and not eloquence, and not sincerity, is where your audit has to bite. Confidence has never been cheaper to manufacture. Evidence remains stubbornly expensive, because reality has to cooperate.

The people who want to move you know this too, and they have noticed that "where are the receipts" is catching on. So the sophisticated ones no longer skip the receipt. They fake its presence.

## Chaff

The word deserves a moment, because it is doing more work than it appears to. In a field, chaff is the husk that threshing leaves behind: worthless, but honest about it. The military borrowed the word for something far less honest. When a missile locks onto an aircraft, the pilot can eject a cloud of cut metallic strips engineered to look, to the missile's radar, exactly like the aircraft itself. The missile was homing on something real. It spends itself on a cloud of nothing, and the real target flies on. That is the sense I mean here.

In your feed, it looks like a citation delivered with total confidence, where no study is actually linked, and where the study, when you finally dig it out, says something quieter or different. It looks like a number with no denominator: something is up forty per cent, but of what, since when, measured how. It looks like a screenshot with no source, a quote with no date, "sources say" with no sources. And in its grandest form it looks like a document so thick that its sheer weight feels like proof, pages and pages, most of them redacted or beside the point, presented with ceremony so that the theatre of showing gets mistaken for the substance of proof.

That is chaff: the shape of evidence, manufactured to satisfy the auditor without feeding it anything. An empty hand held up as though it were full, betting that you will admire the gesture and never look in the palm.

The bet is usually a good one, for a reason with a name. Brandolini's law, the bullshit asymmetry principle, observes that refuting nonsense takes an order of magnitude more effort than producing it. One confident sentence can take a careful person a week to dismantle properly, by which time the parade is three towns away. And notice that the chaff did not need to survive that audit. It only needed to receive it, because every hour of scrutiny it soaks up is an hour that never reaches the real target. The flood of chaff is not laziness or accident. It is a strategy, and it works on intelligent people precisely because they are too busy to audit everything and too trusting to audit the things that please them.

## When absence is sold as proof

One trap left, and it is the cleverest. When you finally ask for the receipt and none appears, a ready-made conclusion is handed to you: the very fact that it is hidden proves how damning it must be. The redactions become the evidence. The silence becomes the smoking gun.

Sometimes things really are hidden, so you cannot simply reverse the rule and treat every gap as innocent. What you need is a single clean discriminator, and here it is. A real receipt survives being handed to someone who wants you to be wrong. It can be checked by a person on neither side, and it stays standing when they check it. Chaff cannot survive that. Chaff needs you friendly, hurried, or already convinced. So the test is not "am I being shown a lot," and it is not "is something being withheld." The test is: would this survive an unfriendly audit? If it only holds up among people who already agree, it was never a receipt. It was a flag you were invited to salute.

Notice that my 128K failed exactly this test. It survived beautifully among friendly company, meaning me. It lasted about four seconds against the configuration file. Your supermarket receipt, by contrast, is the genuine article: inspected by a man paid to assume the worst of you, and still standing.

## The test that costs something

Everything above is easy to aim at your opponents, and that is the final trap, the one that swallows the whole tool. Anyone can demand receipts from the other side. It feels like rigour, and it is often just tribalism wearing rigour's coat.

So here is the move that turns this from a weapon into an instrument. Take the belief you would least like to be wrong about, the one where the question itself feels slightly offensive, and ask where its receipts are. Then watch what you do. If you find yourself reaching for the story instead of the evidence, for how obviously true it is, how everyone sensible knows it, how only a bad person would ask, then you have located the exact spot where your auditor is asleep. It is not across the room. It is in your own chair.

I should tell you that this essay went through that test itself. The first draft was fluent, well shaped, and agreed with everything I already believed, and I read it a dozen times feeling nothing but agreement. It took another reader to point out that my essay about receipts did not contain a single receipt. Every claim in it was assertion, confidently delivered: exactly the produce it warned against. It had read perfectly to me because it agreed with me, which is the whole disease. The version in front of you exists because that audit stung, and I sat with the sting, and then went and got the receipts.

That sting, the flinch when your own side is asked to show its working, is the most valuable signal you will ever get. Not because the cherished belief is necessarily false, but because a belief you cannot bear to audit is being held for reasons that have nothing to do with whether it is true, and that is the one condition every propagandist in history has relied on.

## The equipment

You do not need to become a permanent sceptic, corroding every pleasure, unable to enjoy a film or trust a friend. You need a reflex, switched on at the same four moments the companion essay named: when someone is asking you to believe, to fear, to buy, or to vote. Four questions do the work. Am I being shown the thing itself, or only a description of it? Would this survive an unfriendly audit by someone who wants me to be wrong? Is a missing receipt being sold to me as proof of a cover-up? And the one that costs something: do I ever ask any of this of my own side?

That is the whole kit. It will not make you immune; nothing will, and the companion essay explains why. But the first time you catch a piece of chaff you were about to swallow, and better still the first time you catch one of your own, the habit begins to feed itself.

I was sure it was 128K. The log said 120K. A story asks only to be believed. A receipt asks to be checked. At the moments that matter, learn to tell which one you are holding.

---

*Companion to [The Story Doesn't Care If It's True](01-the-story-doesnt-care.md) and [The Storytelling Framework That Turns Presentations Inside Out](00-storytelling-framework.md). Part of the [Storytelling and Psychology repository](https://github.com/marksunner/storytelling-psychology) by Mark Sunner.*
