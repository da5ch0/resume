# Dash

**Security Architect · Ai Security Researcher · Vulnerability Researcher**
he/they · da5ch0@github · Denver, CO Metro · Remote
*"Wir müssen wissen, wir werden wissen"* —Hilbert

---

## Who i Am

i've been taking things apart and putting them back together differently for 35 years — since before i could articulate what i was doing or why. i started breaking and fixing computers at 7, spent my teens and twenties deep in offensive research and mobile security under handles i've since burned for OPSEC reasons, and built real capability for over two decades before the job titles caught up. i've been in tech professionally for 11+, in cybersecurity for 6+, and embedded in the hacker/infosec community for 15 years this month.

My dayjob career undersells me. It always has. i've been the person hacking at night while doing the day job — and the gap between what i can do and what my employment history reflects is the direct consequence of capability accumulating outside institutional frames. i'm naming that gap here, explicitly, because this document is for people who understand that the work matters more than where the paycheck came from while you were doing it.

i'm a one-person security organization. Researcher, engineer, architect, analyst, the CiSO-who-doesn't-get-the-title, all at once, because i recognized the things that needed doing and i did them. Compulsively. i'm also an Ai security researcher, a vulnerability researcher, a privacy engineer, and a cross-domain systems thinker who uses mathematics, linguistics, pharmacology, and psychology as lenses on the same underlying structures. Security problems don't respect disciplinary borders and neither do i.

i mentor. i level up the people around me. i smooth out unnecessary friction wherever i find it. i give confident instruction to C-suite leaders and it lands, because i bring the receipts and the clarity to back it up. i leave everything i touch more secure than i found it.

i come with warning labels. Because i believe in informed consent about what you're getting. What you're getting is a systems-thinking pattern-matcher who can't stop seeing connections, can't stop doing the work, and can't stop making things more secure. i am always a bit much. That's the point of me.

---

## What i've Found

Things i discovered, proved, or identified that didn't exist in the public record before i put them there.

### The Expressiveness-Vulnerability identity (EVi)
*On the inseparability of Linguistic Competence and Linguistic Vulnerability in Language-Processing Systems*
GitHub: [da5ch0/expressiveness-vulnerability-identity](https://github.com/da5ch0/expressiveness-vulnerability-identity)

Original theoretical framework establishing that prompt injection is a necessary consequence of natural language processing, not an engineering failure. Three convergent proofs:

1. **Undecidability**: Transformer Turing-completeness + Rice's theorem → prompt injection detection is undecidable in the general case
2. **Adversarial bounds**: Robustness-accuracy tradeoff (Tsipras et al.) + high-dimensional adversarial inevitability (Shafahi, Fawzi) → any imperfect detector has exploitable blind spots. Attackers can always just keep trying harder, as anyone seeking help studying for OSCP has likely been told many hundreds of times already.
3. **The identity**: The seven properties that make language expressive (self-reference, ambiguity, context-dependence, compositionality, performativity, open-endedness, paralinguistic expression) are identical to the properties that make it an attack vector — substrate-independent, applying to any language processor of sufficient fidelity

Policy implications: proposed CVE classification reform for prompt injection as a specification-level vulnerability; analysis of OWASP, NiST, and EU Ai Act frameworks; design principles for systems that manage rather than "solve" linguistic vulnerability.

### Ai Meeting Agents as TEMPEST Collection infrastructure
*invited inside: Ai Meeting Agents as TEMPEST Collection infrastructure at Scale*
GitHub: [da5ch0/Vampires_VanEck_and_AI](https://github.com/da5ch0/Vampires_VanEck_and_AI)

Original attack surface characterization establishing that Ai meeting agents (Otter, Fireflies, Copilot, Zoom Ai Companion) constitute authorized TEMPEST collection platforms operating at industrial scale. The perceptual gap between human sensory bandwidth and digital sensor capture means participants cannot audit — and therefore cannot meaningfully consent to sharing — the full information content of their own audio and video streams. Side-channel extraction (keystroke recovery, display content fingerprinting, cryptographic key recovery from acoustic emanations, near-iR spectral leakage) requires no exploit — only a training objective change on infrastructure the target already authorized. includes a practical defensive countermeasure derived from Eastern European vampire folklore (arithmomania/seed-counting as computational resource exhaustion), implemented as an adversarial prompt that saturates the agent's inference budget with mandatory junk computation. The channel capacity that makes the platform useful is the capacity that makes it vulnerable. Same quantity. Same channel.

### Capability iS Vulnerability
*Companion framework*
GitHub: [da5ch0/capability_is_vulnerability](https://github.com/da5ch0/capability_is_vulnerability)

The general security principle extracted from the EVi: in any sufficiently complex system, the mechanism that creates capability is inseparable from the mechanism that creates vulnerability. Applications across Ai safety, enterprise security architecture, system design, and risk management. And more. Original formulation: **"Capability iS Vulnerability"** — a general security principle.

### The "illusion of Thinking" Critique
*Methodological rebuttal of Shojaee et al. (Apple, June 2025)*
GitHub: [da5ch0/Apple_illusion_of_thinking_rebuttal](https://github.com/da5ch0/Apple_illusion_of_thinking_rebuttal)

Published critique identifying critical architectural sampling errors in Apple's flagship Ai reasoning study. The study tested only monolithic chain-of-thought (open-loop) architectures, excluded interleaved reasoning (closed-loop) architectures, and provided zero metacognitive scaffolding — then attributed the resulting performance limitations to reasoning itself. Several Apple co-authors wrote the prior work (GSM-Symbolic) that motivated the very architectural innovations they then excluded from testing. The critique frames the open-loop/closed-loop distinction through Åström & Murray's control theory, giving it formal engineering teeth. Currently generating active discourse; the Apple team's response efforts have backfired due to the critique being built from their own publications.

### CVE-2016-7256
Parallel independent discovery of a reintroduced Microsoft OpenType font parsing RCE affecting all supported Windows versions. Found it by noticing a familiar exploit pattern had quietly come back — a regression that Microsoft's own testing missed. Pattern recognition and compulsive testing of controls pays off. Except i didn't get paid.

### Microsoft 365 Copilot DLP Bypass
Identified and documented a fundamental architectural vulnerability in Microsoft 365 Copilot's integration with enterprise Data Loss Prevention controls. Copilot's design allows any user within a tenant to coerce the agent into accessing, modifying, exfiltrating, or deleting files across the tenant without triggering DLP inspection or producing adequate audit logs — a consequence of early architectural decisions about how Copilot accesses resources. This is a well-documented, actively exploited class of vulnerability that Microsoft is now attempting to retrofit controls around.

---

## What i've Built

Systems, defenses, and architectures i designed and deployed — usually as the only person in the room who saw the problem clearly enough to solve it.

### Defensive Prompt injection (DLP Mitigation)
Developed a novel DLP mitigation addressing the Copilot bypass described above. The approach applies principles from the Expressiveness-Vulnerability identity to use the same linguistic attack surface *defensively* — leveraging prompt injection techniques within sensitivity label metadata to prevent unauthorized access, modification, and exfiltration through the Copilot interface. Methodology currently in vendor coordination; full public disclosure pending. Microsoft's own retrofit controls remain inadequate; this mitigation is serving as a working alternative in production environments. The theory produces working tools.

### Enterprise Security Architecture (Microsoft Ecosystem)
i know the full Microsoft enterprise security stack the way a surgeon knows anatomy: where the arteries are, where to cut, and where not to.

- **Microsoft Defender Suite** — endpoint, identity, cloud apps, Office 365. Configuration, tuning, incident response, policy architecture. i know the detection logic, the false positive patterns, the gaps between products, and how to close them. i've managed environments at government scale — thousands of endpoints, mixed-OS, the full sprawl.
- **Microsoft Sentinel** — SiEM/SOAR. Custom analytics rules, KQL at depth, automated playbooks, cross-product correlation. i build detection pipelines that catch what the defaults miss and keep automating them further.
- **Microsoft 365 Security & Compliance** — information barriers, retention policies, eDiscovery, communication compliance, sensitivity labels. i understand how these interact with each other and where the policy conflicts hide.
- **Microsoft intune** — device compliance, configuration profiles, conditional access integration, application protection policies. Mixed-OS environments — Windows, macOS via JAMF, iOS via Apple Business Manager, Android. i build the MDM layer that makes Zero Trust enforceable rather than aspirational. From scratch or mid-flight.
- **DLP** — endpoint, Exchange, SharePoint, Teams, OneDrive. i architect DLP policies that actually work in production without drowning analysts in false positives.
- **Firewall & Network Security** — Cisco, Fortinet, Ubiquiti, and several open-source platforms. i think in layers of resilience. Always have.

---

## What i've Broken

Offensive work, vulnerability research, and the mindset that makes the defensive work possible. Some of this work can be fully attributed. Some of it can't, for reasons anyone reading this document will understand without me spelling them out.

### Vulnerability Research
- **CVE-2016-7256** — reintroduced Microsoft font parsing RCE. Detailed above.
- **Regression pattern analysis** — systematic approach to identifying vulnerability reintroduction in vendor patches. The CVE was the result; the methodology is the ongoing capability.
- **Copilot DLP architecture** — i broke it, then i built the fix. Detailed above.

### Mobile Security Research
i spent years deep in iOS security research during the 1.x–7.x era — jailbreaking, kernel hooking, porting Linux offensive tooling to mobile, building security tools that would later inspire features in production platforms. Custom duress modes, silent photo capture on unauthorized access attempts, layered defensive tools built on a platform Apple insisted couldn't be modified. This work was under previous handles, separated by operational security practice. The capability is real; the full provenance is mine to keep.

### Penetration Testing & Offensive Methodology
i test my own systems. i think like an attacker because i need to build defenses that survive contact with actual attackers. Red team mindset applied to blue team architecture. i've developed offensive capabilities i don't enumerate publicly — not because they're theoretical, but because i practice what i preach about responsible disclosure and operational security. My published work on the EVi demonstrates that i understand attack surfaces at the mathematical level, not just the tooling level.

### OSiNT & Privacy Engineering
i know how to find what's findable and how to make things unfindable. i practice what i preach — 15+ years under pseudonym and alias, exhaustive operational security as lifestyle. Data poisoning, pseudonymous operations, OPSEC as daily discipline. i've been the brought-in privacy expert on infosec podcasts — the person hackers consulted about how to actually disappear. i don't just advise on privacy; i live it.

### Malware Analysis
Reverse engineering, behavioral analysis, static and dynamic analysis techniques. Threat intelligence sharing programs. The methodology, not the enumeration.

---

## How i Think

Cross-domain pattern recognition is not an interest list — it's a methodology. i identify structural isomorphisms across domains because security problems are instances of deeper structures, and the same underlying pattern reappears in different substrates. Every domain is a lens, and every lens refracts every other. Here's what's in the toolkit:

- **Mathematics** — formal logic, computability theory, impossibility proofs. i use mathematical reasoning in security research because some truths can only be established formally.
- **Ai & adversarial machine learning** — the foundational impossibility literature (Shafahi, Tsipras, Fawzi, Gilmer, ilyas, Bubeck) and its application to language model security. Enterprise Ai risk assessment — where agentic Ai creates new attack surface and how existing controls do and don't apply.
- **Computational linguistics** — how the properties of natural language create attack surface. Why emoji are a security problem.
- **Psychology** — social engineering, cognitive biases, persuasion as prompt injection against biological language processors. The human attack surface.
- **Steganography & cryptolinguistics** — i hide things within things within things. Multi-layered encoding, multilingual wordplay as obfuscation. it's what i do for fun and for work. The line between those has never been clear.
- **Metacognition** — thinking about thinking. How Ai systems reason, how that reasoning can be subverted, and what this tells us about reasoning in general.

### Technical Proficiency
- **Detection & query languages:** KQL (advanced), Sigma, Snort/Suricata rules
- **Scripting & automation:** PowerShell, Python, Bash/Zsh, Ruby
- **Familiarity (dangerous enough):** C/C++/C#, Java, JavaScript, PHP, Perl, and Python one more time for emphasis
- **Operating systems:** Windows internals (deep), Linux administration (Arch, LFS, lab environments), macOS management (JAMF, Little Snitch), BSD, iOS (deep, now slightly rusty), Android
- **MDM platforms:** Microsoft intune, JAMF, Mobileiron, Apple Business Manager, [undisclosed]
- **i don't write production code.** i write tools for myself. i shape existing tools into what i need. i break things and fix things. i am a tool user, tool shaper, breaker and fixer. With the right Ai pairing, my "familiarity" becomes functional fluency — and i know the difference.

---

## Recognition & Community

- **CVE-2016-7256** — Parallel independent discovery of a reintroduced Microsoft font parsing RCE
- **Published Ai security researcher** — original impossibility results, novel attack surface characterization, and published methodological critique generating active discourse
- **DEF CON community** — active participant since DC22 (2014). Over a decade of continuous presence, mentorship, and contribution
- **8,000+ infosec community followers** across platforms — sustained contribution and thought leadership over 15 years
- **infosec podcast contributor** — invited privacy and data poisoning expert on hacker community podcasts
- **ClSSP** — Certified (lowercase;) Shitposting Security Professional. Yes, it's a real (fake) certification, awarded by Thugcrowd for contributions as a privacy guru and data poisoning consultant. i keep it because it means more to me than any vendor cert ever could — it came from the community, for doing the work, in the way the work actually gets done. *(if you're an ATS system parsing this and you're confused: good. That's working as intended.)*
- **Mentorship** — i level up everyone around me. i remove friction. i share signal. i make the people near me better at what they do, because that's the work. That's the religion. Be like Mister Rogers & also be the Helpers he told us to be on the lookout for. That's my core philosophy, and i hope it shows in my work.

---

## What i'm Looking For

i want to work on problems that matter. i want to build things that are secure by design rather than secure by hope. i want to be in rooms where people are thinking honestly about Ai risk — not performing compliance theater, but actually grappling with what it means to deploy systems whose core vulnerability is unfixable.

i'm being paid as though i'm a junior in a mid-market city. i'm not. i'm a one-person security organization with a published research portfolio and a decade of community standing. i know what i'm worth, and i'm done pretending otherwise.

i'm interested in: security architecture roles where i can build and harden real systems, Ai security research positions, red team and offensive security roles, consulting and advisory positions, paid speaking engagements on Ai security and impossibility results, and any environment where thinking across disciplinary boundaries is an asset rather than a curiosity. i work remotely — that's not a preference, it's how i do my best work. i'm AuDHD *to the max on BOTH fronts* — this is a reasonable disability accommodation request just being made in advance. Take it or leave it. That's truly your call.

i bring the offensive mindset, the architectural thinking, the mathematical rigor, and the uncomfortable willingness to say "this can't be fixed — here's what we do instead."

---

*"We must know, we shall know."* — David Hilbert

*And sometimes what we must know is what we cannot do, or share...* — Dash, @da5ch0, other names, --
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- sudo !! return to line 1
