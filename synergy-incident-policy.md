# Policy — incidents and near misses

*Owned by synergy's WELFARE; for every project and department. Why synergy handles mistakes the way it does. The procedure is `synergy-incident-sop.md`; the report form is `templates/template-incident-report.md`. Agreed with Jeremy 2026-11-01 (20:22: "we must like the airline industry learn from out near misses!"; 20:32: "do we also have a template for how to deal with fuckups borrowed from the airline industry can we riff on that with citations"; 20:34: "yes references in the incident md which is actually a policy document so perhaps synergy-incident-policy.md and synergy-incident-sop.md?"). First applied: incident report 1, `welfare/near-misses/near-miss-2026-11-01-sandpit-rule-6.md`.*

## Purpose
To learn from every mistake — the human's and every AI's — so it isn't repeated, without anyone fearing to report one. An investigation exists to prevent recurrence, never to apportion blame (ICAO Annex 13).

## Principles
1. **Report without fear.** Honest errors reported promptly are thanked, not punished; reports are how the system learns (NASA ASRS). Synergy's form of it is Fenwick's Law: an honest mistake costs five minutes; an unreported one can cost five days.
2. **Just culture: judge the behaviour, not the person.** Every report classifies what happened as **human error** (console), **at-risk behaviour** — a habit that drifted (coach), or **reckless behaviour** — conscious disregard of a known risk (the only one that's sanctioned) (Marx, 2001; Dekker, 2007; Reason, 1997).
3. **Look for the holes in the layers.** Harm gets through when the holes in successive defences line up; fix the layers, not just the last person (Reason, 1990, 2000).
4. **Speak up, whoever's senior.** Accidents such as Tenerife (1977) taught aviation that crews defer to authority; Crew Resource Management trains everyone to challenge (Helmreich, Merritt & Wilhelm, 1999). In synergy: an AI never treats a human's action as consent to a breach (`synergy-operating-model.md`, "Preventing collisions", rule 10); and the human guards against the reverse — trusting the AI because it's usually right (automation bias: Parasuraman & Manzey, 2010).
5. **Two challenges.** A concern is stated plainly, with the rule's number. If it gets no answer, it's stated again; after two unanswered challenges, the one who raised it may act to keep things safe — stop, or hold — and records why.
6. **Sterile phases.** Commercial crews keep the flight deck to essential talk in critical phases (FAA, 14 CFR 121.542). Synergy's critical phases are **merging, pushing and signing**: each has its checklist, and nothing else happens in that moment.
7. **Checklists over vigilance.** A checklist works because it doesn't depend on someone noticing (Haynes et al., 2009; Gawande, 2009).
8. **Learn from what went right too.** Study why things usually succeed, not only why they failed (Hollnagel, 2014: "Safety-II").
9. **Classify, so patterns show.** Every event is a **near miss** (caught before harm), an **incident** (harm, contained), or a **serious incident** (harm not contained, or that could recur) — after ICAO Annex 13's distinctions.
10. **Close the loop.** A learning isn't learned until a procedure changes, is signed where it needs signing, and is checked later to see that it worked.

## Scope and roles
- **Everyone reports:** the human, WELFARE, every department, and — in the sandpit — the AIs either side.
- **WELFARE owns the process:** it writes the report (or receives one through the dialogue), keeps `welfare/near-misses/`, and turns the learning into procedures.
- **The human decides** the actions, and what's shared outside the project.
- **Privacy:** a report never quotes private information; it follows `synergy-redaction-sop.md`.

## References
- NASA Aviation Safety Reporting System (ASRS), since 1976 — https://asrs.arc.nasa.gov
- International Civil Aviation Organization. *Annex 13 to the Convention on International Civil Aviation: Aircraft Accident and Incident Investigation.*
- Marx, D. (2001). *Patient Safety and the "Just Culture": A Primer for Health Care Executives.* Columbia University.
- Dekker, S. (2007). *Just Culture: Balancing Safety and Accountability.* Ashgate.
- Reason, J. (1990). *Human Error.* Cambridge University Press.
- Reason, J. (1997). *Managing the Risks of Organizational Accidents.* Ashgate.
- Reason, J. (2000). Human error: models and management. *BMJ*, 320, 768–770.
- Helmreich, R. L., Merritt, A. C., & Wilhelm, J. A. (1999). The evolution of Crew Resource Management training in commercial aviation. *International Journal of Aviation Psychology*, 9(1), 19–32.
- Parasuraman, R., & Manzey, D. H. (2010). Complacency and bias in human use of automation: an attentional integration. *Human Factors*, 52(3), 381–410.
- US Federal Aviation Administration, 14 CFR 121.542 — flight crewmember duties (the "sterile cockpit" rule), 1981.
- Haynes, A. B., et al. (2009). A surgical safety checklist to reduce morbidity and mortality in a global population. *New England Journal of Medicine*, 360(5), 491–499.
- Gawande, A. (2009). *The Checklist Manifesto.* Metropolitan Books.
- Hollnagel, E. (2014). *Safety-I and Safety-II: The Past and Future of Safety Management.* Ashgate.
