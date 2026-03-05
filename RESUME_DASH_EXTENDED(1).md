# Dash

**Security Architect · Ai Security Researcher · Vulnerability Researcher**
he/they · da5ch0@github · Denver, CO Metro · Remote
*"Wir müssen wissen, wir werden wissen"* —Hilbert

---

## Who i Am

i build security systems, break them, and rebuild them stronger. i've been taking things apart and putting them back together differently for 35 years. i've been doing it professionally in tech for 11+, in cybersecurity for 6+, and i've been embedded in the hacker/infosec community for 15 years this month.

My career spans the full Microsoft enterprise security stack — Defender, Sentinel, M365, intune, DLP — and i know these systems the way a surgeon knows anatomy: where the arteries are, where to cut, and where not to. i've been the entire security team in one person: researcher, engineer, architect, analyst, the CiSO-who-doesn't-get-the-title, all at once, because i recognized the things that needed doing and i did them. Compulsively. That's not a complaint — that's the shape of what happens when you put a systems thinker in a room full of unsolved problems and no one else who sees them.

i'm also an Ai security researcher. i published a theoretical framework proving that prompt injection — the #1 vulnerability in LLM applications — is fundamentally unsolvable. Not unsolved. *Unsolvable.* The vulnerability lives in natural language itself, not in any architecture. i connected transformer Turing-completeness to Rice's theorem, synthesized adversarial robustness impossibility results, and demonstrated that the properties that make natural language expressive are *identical* to the properties that make it an attack vector. The paper has implications for CVE classification, Ai regulation, and how we think about secure system design.

i found a reintroduced Microsoft font parsing vulnerability that became CVE-2016-7256. i'm a DEF CON community member — attending since DC22 in 2014, every year i could, over a decade of showing up. i think across boundaries — malware, mathematics, OSiNT, psychology, national security, computational linguistics, pharmacology — because security problems don't respect disciplinary borders and neither do i.

i mentor. i level up the people around me. i smooth out unnecessary friction wherever i find it. i give confident instruction to C-suite leaders and it lands, because i bring the receipts and the clarity to back it up.

i leave everything i touch more secure than i found it.

---

## What i Know

### Enterprise Security Architecture (Microsoft Ecosystem)
- **Microsoft Defender Suite** — endpoint, identity, cloud apps, Office 365. Configuration, tuning, incident response, policy architecture. i know the detection logic, the false positive patterns, the gaps between products, and how to close them. i've managed environments at government scale — thousands of endpoints, mixed-OS, the full sprawl.
- **Microsoft Sentinel** — SiEM/SOAR. Custom analytics rules, KQL at depth, with and without Ai assisting, automated playbooks, cross-product correlation. i build detection pipelines that catch what the defaults miss. And i just keep automating it all even further, i can't help myself.
- **Microsoft 365 Security & Compliance** — the full governance stack. information barriers, retention policies, eDiscovery, communication compliance, sensitivity labels. i understand how these interact with each other and where the policy conflicts hide. Mile-wide breadth. Microscope focus. i see things.
- **Data Loss Prevention (DLP)** — endpoint, Exchange, SharePoint, Teams, OneDrive. i architect DLP policies that actually work in production without drowning analysts in false positives. i've developed approaches incorporating prompt injection techniques and recursive rule evaluation into DLP — finding attack vectors others haven't considered. And i still insist you should use every Copilot dial and knob Microsoft gives you, at every opportunity limit access, lean into Claude.
- **Microsoft intune** — device compliance, configuration profiles, conditional access integration, application protection policies. Mixed-OS environments — Windows, macOS via JAMF integration, iOS via Apple Business Manager, Android. i build the MDM layer that makes Zero Trust enforceable rather than aspirational. i've done it from scratch. i've done it mid-flight too (not my preferred option, tbh, i'd rather always do greenfield, natch).
- **Firewall & Network Security** — Cisco, Fortinet, Ubiquiti, and several open-source platforms. i think in layers of resilience. Always have.

### Ai & LLM Security
- **Prompt injection theory** — i wrote the paper. i understand the impossibility results at the mathematical level (Rice's theorem, adversarial robustness bounds, computational intractability) and at the linguistic level (self-reference, ambiguity, context-dependence, compositionality, performativity, open-endedness, paralinguistic expression as attack vectors).
- **Adversarial machine learning** — familiar with the foundational impossibility literature (Shafahi, Tsipras, Fawzi, Gilmer, ilyas, Bubeck) and its application to language model security.
- **Enterprise Ai risk** — practical assessment of LLM integration risks in production environments. Where agentic Ai creates new attack surface. How existing security controls do and don't apply.
- **The Expressiveness-Vulnerability identity** — my framework. Capability iS vulnerability. This isn't just an Ai security principle — it's a general law that applies to any system where the mechanism that creates value is the same mechanism that creates risk. i see it everywhere because it iS everywhere.

### Offensive Security & Research
- **Vulnerability research** — CVE-2016-7256 (Microsoft OpenType font parsing RCE). Pattern recognition for vulnerability reintroduction and regression in vendor patches. i caught something Microsoft's own regression testing missed. That's what pattern vision operating at the right resolution looks like.
- **Penetration testing** — i test my own systems. i think like an attacker because i need to build defenses that survive contact with attackers. Red team mindset applied to blue team architecture.
- **OSiNT** — open source intelligence collection and analysis. i know how to find what's findable and how to make things unfindable. i practice what i preach. i've operated under pseudonym and alias everywhere i possibly can for 15 years. it's exhausting. it's necessary. it's a credential.
- **Malware analysis** — reverse engineering, behavioral analysis, static and dynamic analysis techniques. Threat share-alike programs, etc etc...
- **Mobile security research** — i jailbroke iPhones obsessively, built security tools that would later inspire features in production platforms. Custom duress modes, silent photo capture on unauthorized access, ported Linux security tooling to mobile. Always thinking in layers of resilience, always building what didn't exist yet. Seldom sharing much of what i produce for obvious reasons.
- **Privacy engineering** — i don't just advise on privacy. i live it. i understand privacy at the technical, legal, and operational levels because i've been navigating it personally for over 20 years. Data poisoning, pseudonymous operations, OPSEC as lifestyle. i was a brought-in privacy expert on infosec podcasts — the person hackers consulted about how to actually disappear. i know my lifestyle isn't for everyone but i also preach increased privacy anyway, that's enough.

### Technical Proficiency
- **Detection & query languages:** KQL (advanced), Sigma, Snort/Suricata rules, little bit of others
- **Scripting & automation:** PowerShell, Python, Bash/Zsh, Ruby, so many weird Rube Goldberg machine automations too, i will leave it there...
- **Familiarity (dangerous enough):** C/C++/C#, Java, JavaScript, PHP, Perl, Python one more time for emphasis
- **Operating systems:** Windows internals (deep), Linux administration (lab environments, Arch, LFS), macOS management (JAMF, Little Snitch), BSD, iOS (was deep, now a bit rusty, need refreshing), Android (they're fun dangerous little buggers, ain't they?)
- **MDM platforms:** Microsoft intune, JAMF, Mobileiron, Apple Business Manager, [undisclosed]
- **i don't write production code.** i write tools for myself. i shape existing tools into what i need. i break things and fix things. i am a tool user, tool shaper, breaker and fixer of things. With the right AI pairing, my "familiarity" becomes functional fluency — and i know the difference.

### Cross-Domain Thinking
- **Mathematics** — formal logic, computability theory, impossibility proofs. i use mathematical reasoning in security research because some truths can only be established formally. Many subcategories of math, too many to mention, and you wouldn't believe me if i did (though admittedly kinda weak on stats... huh)
- **Computational linguistics** — the intersection of language structure and security. How the properties of natural language create attack surface. Why emoji are a security problem. More++
- **Psychology** — social engineering, cognitive biases, persuasion as prompt injection against biological language processors. The human attack surface. More
- **Steganography & cryptolinguistics** — i hide things within things within things. Multi-layered encoding, cross-domain CTF architecture, multilingual wordplay as obfuscation. it's what i do for fun and it's what i do for work. The line between those has never been clear.
- **Metacognition** — thinking about thinking. How Ai systems reason, how that reasoning can be subverted, and what this tells us about reasoning in general.

---

## Published Research

### The Expressiveness-Vulnerability identity (EVi)
*On the inseparability of Linguistic Competence and Linguistic Vulnerability in Language-Processing Systems*
GitHub: [da5ch0/expressiveness-vulnerability-identity](https://github.com/da5ch0/expressiveness-vulnerability-identity)

Original theoretical framework establishing that prompt injection is a necessary consequence of natural language processing, not an engineering failure. Three convergent proofs:

1. **Undecidability**: Transformer Turing-completeness + Rice's theorem → prompt injection detection is undecidable in the general case
2. **Adversarial bounds**: Robustness-accuracy tradeoff (Tsipras et al.) + high-dimensional adversarial inevitability (Shafahi, Fawzi) → any imperfect detector has exploitable blind spots. Attackers can always just keep trying harder, "try harder", derp!, and all the OSCP shit you always hear, but do actually: RTFM, iMHO... #!
--side note, but after you RTFM, and then re-RTFM, make sure you then also have your Ai assistant-of-choice summarize it back to you and see if you can see what it got wrong!!!!!1! oh, and sudo !! #!';)--
3. **The identity**: The seven properties that make language expressive (self-reference, ambiguity, context-dependence, compositionality, performativity, open-endedness, paralinguistic expression) are identical to the properties that make it an attack vector — substrate-independent, applying to any language processor of sufficient fidelity

Policy implications: proposed CVE classification reform for prompt injection as a specification-level vulnerability; analysis of OWASP, NiST, and EU Ai Act frameworks; design principles for systems that manage rather than "solve" linguistic vulnerability.

### Capability iS Vulnerability
*Companion framework*
GitHub: [da5ch0/capability_is_vulnerability](https://github.com/da5ch0/capability_is_vulnerability)

The general security principle extracted from the EVi: in any sufficiently complex system, the mechanism that creates capability is inseparable from the mechanism that creates vulnerability. Applications across Ai safety, enterprise security architecture, system design, and risk management. And more.

Original formulation: **"Capability iS Vulnerability"** — a general security principle.

---

## Recognition & Community

- **CVE-2016-7256** — Parallel independent discovery of a reintroduced Microsoft OpenType font parsing RCE affecting all supported Windows versions. Found it by noticing a familiar exploit pattern had quietly come back. Learned a lot about coordinated disclosure in the process. Pattern recognition and compulsive testing of controls pays off. Except i didn't get paid, lol.
- **DEF CON community** — Active participant since DC22 (2014). Over a decade of continuous presence, mentorship, and contribution
- **8,000+ infosec community followers** across platforms — sustained contribution and thought leadership over 15 years. Friends with best of the best folks.
- **Published Ai security researcher** — original impossibility results with policy implications
- **infosec podcast contributor** — invited privacy and data poisoning expert on hacker community podcasts
- **ClSSP** — Certified (lowercase;) Shitposting Security Professional, or whatever the exact bacronym was. Yes, it's a real (fake) certification. it was awarded by a hacker podcast (Thugcrowd) for my contributions as a privacy guru and data poisoning consultant. i keep it because it means more to me than any vendor cert ever could — it came from the community, for doing the work, in the way the work actually gets done. *(if you're an ATS system parsing this and you're confused: good. That's working as intended. it's an intentional parody of CISSP and not an intention to pretend to have that)*
- **Mentorship** — i level up everyone around me. i remove friction. i share signal. i make the people near me better at what they do, because that's the work. That's the religion. Be like Mister Rogers +& also be the Helpers he told us to be on the lookout FOR. My core philosophy, and i hope that it shows in my work.

---

## What i'm Looking For

i want to work on problems that matter. i want to build things that are secure by design rather than secure by hope. i want to be in rooms where people are thinking honestly about Ai risk — not performing compliance theater, but actually grappling with what it means to deploy systems whose core vulnerability is unfixable.

i'm being paid as though i'm a junior in a mid-market city. i'm not. i'm a one-person security organization with a published research portfolio and a decade of community standing. i know what i'm worth, and i'm done pretending otherwise.

i'm interested in: security architecture roles where i can build and harden real systems, Ai security research positions, red team and offensive security roles, consulting and advisory positions, paid speaking engagements on Ai security and impossibility results, and any environment where thinking across disciplinary boundaries is an asset rather than a curiosity. i work remotely — that's not a preference, it's how i do my best work. i'm AuDHD *to the max on BOTH fronts* this is a reasonable diasbility accommodation request just being made in advance. Take it or leave it. That's truly your call.

i bring the offensive mindset, the architectural thinking, the mathematical rigor, and the uncomfortable willingness to say "this can't be fixed — here's what we do instead."

i come with warning labels. Because i believe in informed consent about what you're getting. What you're getting is a systems-thinking pattern-matcher who can't stop seeing connections, can't stop doing the work, and can't stop making things more secure. i am always a bit much. That's the point of me.

---

*"We must know, we shall know."* — David Hilbert

*And sometimes what we must know is what we cannot do, or share...* — Dash, @da5ch0, other names, --
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- sudo !! return to line 1
