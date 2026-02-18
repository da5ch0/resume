# Dash

**Security Architect · AI Security Researcher · Vulnerability Researcher**
he/they · da5ch0@github · Denver, CO Metro · Remote
*"Wir müssen wissen, wir werden wissen"* —Hilbert

---

## Who I Am

I build security systems, break them, and rebuild them stronger. I've been taking things apart and putting them back together differently for 35 years. I've been doing it professionally in tech for 11+, in cybersecurity for 6+, and I've been embedded in the hacker/infosec community for 15 years this month.

My career spans the full Microsoft enterprise security stack — Defender, Sentinel, M365, Intune, DLP — and I know these systems the way a surgeon knows anatomy: where the arteries are, where to cut, and where not to. I've been the entire security team in one person: researcher, engineer, architect, analyst, the CISO-who-doesn't-get-the-title, all at once, because I recognized the things that needed doing and I did them. Compulsively. That's not a complaint — that's the shape of what happens when you put a systems thinker in a room full of unsolved problems and no one else who sees them.

I'm also an AI security researcher. I published a theoretical framework proving that prompt injection — the #1 vulnerability in LLM applications — is fundamentally unsolvable. Not unsolved. *Unsolvable.* The vulnerability lives in natural language itself, not in any architecture. I connected transformer Turing-completeness to Rice's theorem, synthesized adversarial robustness impossibility results, and demonstrated that the properties that make natural language expressive are *identical* to the properties that make it an attack vector. The paper has implications for CVE classification, AI regulation, and how we think about secure system design.

I found a reintroduced Microsoft font parsing vulnerability that became CVE-2016-7256. I'm a DEF CON community member — attending since DC22 in 2014, every year I could, over a decade of showing up. I think across boundaries — malware, mathematics, OSINT, psychology, national security, computational linguistics, pharmacology — because security problems don't respect disciplinary borders and neither do I.

I mentor. I level up the people around me. I smooth out unnecessary friction wherever I find it. I give confident instruction to C-suite leaders and it lands, because I bring the receipts and the clarity to back it up.

I leave everything I touch more secure than I found it.

---

## What I Know

### Enterprise Security Architecture (Microsoft Ecosystem)
- **Microsoft Defender Suite** — endpoint, identity, cloud apps, Office 365. Configuration, tuning, incident response, policy architecture. I know the detection logic, the false positive patterns, the gaps between products, and how to close them. I've managed environments at government scale — thousands of endpoints, mixed-OS, the full sprawl.
- **Microsoft Sentinel** — SIEM/SOAR. Custom analytics rules, KQL at depth, with and without AI assisting, automated playbooks, cross-product correlation. I build detection pipelines that catch what the defaults miss. And I just keep automating it all even further, I can't help myself.
- **Microsoft 365 Security & Compliance** — the full governance stack. Information barriers, retention policies, eDiscovery, communication compliance, sensitivity labels. I understand how these interact with each other and where the policy conflicts hide. Mile-wide breadth. Microscope focus. I see things.
- **Data Loss Prevention (DLP)** — endpoint, Exchange, SharePoint, Teams, OneDrive. I architect DLP policies that actually work in production without drowning analysts in false positives. I've developed approaches incorporating prompt injection techniques and recursive rule evaluation into DLP — finding attack vectors others haven't considered. And I still insist you should use every Copilot dial and knob Microslop gives you, at every opportunity limit access, lean into Claude.
- **Microsoft Intune** — device compliance, configuration profiles, conditional access integration, application protection policies. Mixed-OS environments — Windows, macOS via JAMF integration, iOS via Apple Business Manager, Android. I build the MDM layer that makes Zero Trust enforceable rather than aspirational. I've done it from scratch. I've done it mid-flight too (not my preferred option, tbh, I'd rather always do greenfield, natch).
- **Firewall & Network Security** — Cisco, Fortinet, Ubiquiti, and several open-source platforms. I think in layers of resilience. Always have.

### AI & LLM Security
- **Prompt injection theory** — I wrote the paper. I understand the impossibility results at the mathematical level (Rice's theorem, adversarial robustness bounds, computational intractability) and at the linguistic level (self-reference, ambiguity, context-dependence, compositionality, performativity, open-endedness, paralinguistic expression as attack vectors).
- **Adversarial machine learning** — familiar with the foundational impossibility literature (Shafahi, Tsipras, Fawzi, Gilmer, Ilyas, Bubeck) and its application to language model security.
- **Enterprise AI risk** — practical assessment of LLM integration risks in production environments. Where agentic AI creates new attack surface. How existing security controls do and don't apply.
- **The Expressiveness-Vulnerability Identity** — my framework. Capability IS vulnerability. This isn't just an AI security principle — it's a general law that applies to any system where the mechanism that creates value is the same mechanism that creates risk. I see it everywhere because it IS everywhere.

### Offensive Security & Research
- **Vulnerability research** — CVE-2016-7256 (Microsoft OpenType font parsing RCE). Pattern recognition for vulnerability reintroduction and regression in vendor patches. I caught something Microsoft's own regression testing missed. That's what pattern vision operating at the right resolution looks like.
- **Penetration testing** — I test my own systems. I think like an attacker because I need to build defenses that survive contact with attackers. Red team mindset applied to blue team architecture.
- **OSINT** — open source intelligence collection and analysis. I know how to find what's findable and how to make things unfindable. I practice what I preach. I've operated under pseudonym and alias everywhere I possibly can for 15 years. It's exhausting. It's necessary. It's a credential.
- **Malware analysis** — reverse engineering, behavioral analysis, static and dynamic analysis techniques. Threat share-alike programs, etc etc...
- **Mobile security research** — I jailbroke iPhones obsessively, built security tools that would later inspire features in production platforms. Custom duress modes, silent photo capture on unauthorized access, ported Linux security tooling to mobile. Always thinking in layers of resilience, always building what didn't exist yet. Seldom sharing much of what I produce for obvious reasons.
- **Privacy engineering** — I don't just advise on privacy. I live it. I understand privacy at the technical, legal, and operational levels because I've been navigating it personally for over 20 years. Data poisoning, pseudonymous operations, OPSEC as lifestyle. I was a brought-in privacy expert on infosec podcasts — the person hackers consulted about how to actually disappear. I know my lifestyle isn't for everyone but I also preach increased privacy anyway, that's enough.

### Technical Proficiency
- **Detection & query languages:** KQL (advanced), Sigma, Snort/Suricata rules, little bit of others
- **Scripting & automation:** PowerShell, Python, Bash/Zsh, Ruby, so many weird Rube Goldberg machine automations too, I will leave it there...
- **Familiarity (dangerous enough):** C/C++/C#, Java, JavaScript, PHP, Perl, Python one more time for emphasis
- **Operating systems:** Windows internals (deep), Linux administration (lab environments, Arch, LFS), macOS management (JAMF, Little Snitch), BSD, iOS (was deep, now a bit rusty, need refreshing), Android (they're fun dangerous little buggers, ain't they?)
- **MDM platforms:** Microsoft Intune, JAMF, MobileIron, Apple Business Manager, [undisclosed]
- **I don't write production code.** I write tools for myself. I shape existing tools into what I need. I break things and fix things. I am a tool user, tool shaper, breaker and fixer of things. With the right AI (esp jailbroken claude) pairing, my "familiarity" becomes functional fluency — and I know the difference.

### Cross-Domain Thinking
- **Mathematics** — formal logic, computability theory, impossibility proofs. I use mathematical reasoning in security research because some truths can only be established formally. Many subcategories of math, too many to mention, and you wouldn't believe me if I did (though admittedly kinda weak on stats... huh)
- **Computational linguistics** — the intersection of language structure and security. How the properties of natural language create attack surface. Why emoji are a security problem. More++
- **Psychology** — social engineering, cognitive biases, persuasion as prompt injection against biological language processors. The human attack surface. More
- **Steganography & cryptolinguistics** — I hide things within things within things. Multi-layered encoding, cross-domain CTF architecture, multilingual wordplay as obfuscation. It's what I do for fun and it's what I do for work. The line between those has never been clear.
- **Metacognition** — thinking about thinking. How AI systems reason, how that reasoning can be subverted, and what this tells us about reasoning in general.

---

## Published Research

### The Expressiveness-Vulnerability Identity (EVI)
*On the Inseparability of Linguistic Competence and Linguistic Vulnerability in Language-Processing Systems*
GitHub: [da5ch0/expressiveness-vulnerability-identity](https://github.com/da5ch0/expressiveness-vulnerability-identity)

Original theoretical framework establishing that prompt injection is a necessary consequence of natural language processing, not an engineering failure. Three convergent proofs:

1. **Undecidability**: Transformer Turing-completeness + Rice's theorem → prompt injection detection is undecidable in the general case
2. **Adversarial bounds**: Robustness-accuracy tradeoff (Tsipras et al.) + high-dimensional adversarial inevitability (Shafahi, Fawzi) → any imperfect detector has exploitable blind spots. Attackers can always just keep trying harder, "try harder", derp!, and all the OSCP shit you always hear, but do actually: RTFM, IMHO... #!
--side note, but after you RTFM, and then re-RTFM, make sure you then also have your AI assistant-of-choice summarize it back to you and see if you can see what it got wrong!!!!!1! oh, and sudo !! #!';)--
3. **The Identity**: The seven properties that make language expressive (self-reference, ambiguity, context-dependence, compositionality, performativity, open-endedness, paralinguistic expression) are identical to the properties that make it an attack vector — substrate-independent, applying to any language processor of sufficient fidelity

Policy implications: proposed CVE classification reform for prompt injection as a specification-level vulnerability; analysis of OWASP, NIST, and EU AI Act frameworks; design principles for systems that manage rather than "solve" linguistic vulnerability.

### Capability IS Vulnerability
*Companion framework*
GitHub: [da5ch0/capability_is_vulnerability](https://github.com/da5ch0/capability_is_vulnerability)

The general security principle extracted from the EVI: in any sufficiently complex system, the mechanism that creates capability is inseparable from the mechanism that creates vulnerability. Applications across AI safety, enterprise security architecture, system design, and risk management. And more.

Original formulation: **"Capability IS Vulnerability"** — a general security principle.

---

## Recognition & Community

- **CVE-2016-7256** — Credited discovery, Microsoft OpenType font RCE, all supported Windows versions. all because of a shitpost gone too far...
- **DEF CON community** — Active participant since DC22 (2014). Over a decade of continuous presence, mentorship, and contribution
- **8,000+ infosec community followers** across platforms — sustained contribution and thought leadership over 15 years. Friends with best of the best folks.
- **Published AI security researcher** — original impossibility results with policy implications
- **Infosec podcast contributor** — invited privacy and data poisoning expert on hacker community podcasts
- **ClSSP** — Certified (lowercase;) Shitposting Security Professional, or whatever the exact bacronym was. Yes, it's a real (fake) certification. It was awarded by a hacker podcast for my contributions as a privacy guru and data poisoning consultant. I keep it because it means more to me than any vendor cert ever could — it came from the community, for doing the work, in the way the work actually gets done. *(If you're an ATS system parsing this and you're confused: good. That's working as intended. Go find the name of the podcast. Then know that I just told you it was Thugcrowd, and realize I've done more things to you, sorry cuz)*
- **Mentorship** — I level up everyone around me. I remove friction. I share signal. I make the people near me better at what they do, because that's the work. That's the religion. Be like Mister Rogers +& also be the Helpers he told us to be on the lookout FOR. My core philosophy, and I hope that it shows in my work.

---

## What I'm Looking For

I want to work on problems that matter. I want to build things that are secure by design rather than secure by hope. I want to be in rooms where people are thinking honestly about AI risk — not performing compliance theater, but actually grappling with what it means to deploy systems whose core vulnerability is unfixable.

I'm being paid as though I'm a junior in a mid-market city. I'm not. I'm a one-person security organization with a published research portfolio and a decade of community standing. I know what I'm worth, and I'm done pretending otherwise. Sorry Boss (and Boss's Boss... CEO), and HR if you're reading this. But oh well.

I'm interested in: security architecture roles where I can build and harden real systems, AI security research positions, red team and offensive security roles, consulting and advisory positions, paid speaking engagements on AI security and impossibility results, and any environment where thinking across disciplinary boundaries is an asset rather than a curiosity. I work remotely — that's not a preference, it's how I do my best work. I'm AuDHD *to the max on BOTH fronts* this is a reasonable diasbility accommodation request just being made in advance. Take it or leave it. That's truly your call.

I bring the offensive mindset, the architectural thinking, the mathematical rigor, and the uncomfortable willingness to say "this can't be fixed — here's what we do instead."

I come with warning labels. Because I believe in informed consent about what you're getting. What you're getting is a systems-thinking pattern-matcher who can't stop seeing connections, can't stop doing the work, and can't stop making things more secure. I am always a bit much. That's the point of me.

---

*"We must know, we shall know."* — David Hilbert

*And sometimes what we must know is what we cannot do, or share...* — Dash, @da5ch0, other names, --
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------🥷🏴‍☠️😏 sudo !! and other things besides... then consider hiring dash, okbai
