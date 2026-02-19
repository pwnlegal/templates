# UK cyber security legal templates

Open-source engagement documents for UK penetration testers and IASME certification bodies. English law. Ready to use.

Published by [pwn.legal](https://templates.pwn.legal) · Maintained by [Deeptech Legal](https://deeptech.legal)

Draws on concepts from [Cure53/Contracts](https://github.com/cure53/Contracts), [TrustedSec/physical-docs](https://github.com/TrustedSec/physical-docs), [PTES](http://www.pentest-standard.org/), [disclose.io](https://disclose.io), and [Common Paper](https://commonpaper.com).

## Penetration testing

| Template                       | File                                                                                       |
| ------------------------------ | ------------------------------------------------------------------------------------------ |
| MSA                            | [`msa.md`](templates/pentest/msa.md)                                                       |
| SOW                            | [`sow.md`](templates/pentest/sow.md)                                                       |
| Authorisation to test          | [`authorisation-to-test.md`](templates/pentest/authorisation-to-test.md)                   |
| Physical testing authorisation | [`physical-testing-authorisation.md`](templates/pentest/physical-testing-authorisation.md) |
| DPA                            | [`dpa.md`](templates/pentest/dpa.md)                                                       |

Sign the MSA once and attach SOWs per engagement. Drafted from the tester's perspective. Re-testing isn't included by default. Third-party vulnerability information (third-party vulns found during testing) is excluded from confidentiality by default. Insurance clauses are descriptive not prescriptive; specify your actual cover in the SOW. If you need advice about your insurance position, ask us on [Slack](https://pwnlegal.slack.com) or by email: [rich@pwn.legal](mailto:rich@pwn.legal).

## Non-disclosure agreements (NDAs)

The MSA and Standard terms contain mutual confidentiality commitments tailored to the nature of the work. For pre-engagement confidentiality agreements, take a look at the [OneNDA](https://onenda.org) template.

## IASME Certification Bodies

| Template                                     | File                                                                              |
| -------------------------------------------- | --------------------------------------------------------------------------------- |
| Standard terms                               | [`standard-terms.md`](templates/iasme-cb/standard-terms.md)                       |
| Order form                                   | [`order-form.md`](templates/iasme-cb/order-form.md)                               |
| Schedule CE — Cyber Essentials               | [`schedule-ce.md`](templates/iasme-cb/schedule-ce.md)                             |
| Schedule CE+ — Cyber Essentials Plus         | [`schedule-ce-plus.md`](templates/iasme-cb/schedule-ce-plus.md)                   |
| Schedule Cyber Assurance                     | [`schedule-cyber-assurance.md`](templates/iasme-cb/schedule-cyber-assurance.md)   |
| Schedule CB — Cyber Baseline (international) | [`schedule-cb-international.md`](templates/iasme-cb/schedule-cb-international.md) |
| Schedule DCC — Defence Cyber Certification   | [`schedule-dcc.md`](templates/iasme-cb/schedule-dcc.md)                           |
| Schedule IoT Baseline                        | [`schedule-iot-baseline.md`](templates/iasme-cb/schedule-iot-baseline.md)         |
| Schedule IoT Assurance                       | [`schedule-iot-assurance.md`](templates/iasme-cb/schedule-iot-assurance.md)       |
| Schedule Maritime                            | [`schedule-maritime.md`](templates/iasme-cb/schedule-maritime.md)                 |

IASME is a registered trade mark of The IASME Consortium Limited. Cyber Essentials is a registered trade mark of the National Cyber Security Centre (NCSC). These templates are not endorsed by, affiliated with, or authorised by The IASME Consortium Limited or the NCSC.

The Standard Terms are designed to be used together with an Order Form for each engagement, and a Schedule for each certification scheme in scope of the engagement.

For example: CE basic = standard terms + order form + Schedule CE. Add Schedule CE+ for Plus, Schedule DCC for defence, and so on.

Guidance and readiness support are handled within the standard terms and order form, not as a separate schedule. Indicate on each Order Form whether consultation/guidance and certification fees are included, separately charged, or not applicable.

**If you also do standalone penetration testing:** The CB standard terms handle data via clause 7 and do not include a separate DPA: for standard CE basic assessments (questionnaire-based, no system access). For more intensive scanning and testing, consider adopting the pentest DPA.

## Where bespoke advice is recommended

These templates cover the majority of commercial penetration testing and IASME certification engagements. The following scenarios fall outside the safe defaults and should be scoped with specialist legal input.

**Penetration testing:** red team rules of engagement; CBEST, STAR, and TLPT regulatory testing; classified systems and security-cleared work; cross-border and multi-jurisdiction testing; fully autonomous AI testing agents; third-party reliance on pentest reports; government-issued identity documents and KYC pipeline testing.

**IASME certification:** multi-CB arrangements and white-labelled assessment services; managing IASME audit findings that contradict your assessment; DCC Level 3 and CAA ASSURE (NCSC-approved methodologies, bespoke engagement models).

## Adapting these templates

The templates use reasonable defaults. When implementing them for your own practice, the following are areas where the defaults may not suit your circumstances and where the right answer depends on your business model, risk appetite, and client base.

**Liability caps and risk allocation.** The default cap (200% of fees per SOW) is a starting point. The right level depends on your insurance cover, the size and sensitivity of engagements you take on, and your client profile. Caps that sit below your insurance limit might not be enforceable; consider taking legal advice.

**Workforce, subcontracting, and team protection.** The templates permit subcontracting with the tester remaining responsible, but do not include non-solicitation provisions. Whether you need protection against clients recruiting your testers (or vice versa) depends on how your team is structured — employed, contracted, or associate — and the enforceability of such provisions turns on the specific employment or engagement relationship. This is an area where a generic clause is more likely to mislead than to protect.

**Insurance requirements.** The templates are descriptive (specify your cover in the SOW) rather than prescriptive (minimum £X required). If your clients require specific minimum coverage or if you operate under CHECK or CREST, you may need to add mandatory minimums.

**Regulatory and accreditation overlays.** CHECK, CREST, Cyber Scheme, and PCI DSS each impose additional obligations that may need to be reflected in your terms. The SOW includes an accreditation framework field, but firms operating primarily under these frameworks may want dedicated provisions in the MSA.

**YMMV.** Consider what your position might be if the following terms are redlined by clients:

- _Third-party vulnerability disclosure (MSA 10.5)._ The default allows the tester to report third-party vulnerabilities to vendors and CERTs after a coordination process. Clients in financial services, defence, or with sensitive vendor relationships may want to extend the coordination window or require joint disclosure. The 90-day maximum delay is negotiable; the principle that third-party vulnerabilities are not the client's confidential information is not.
- _IP and report sharing (MSA 9)._ Regulated clients may need to share reports with group companies, external auditors, or acquirers beyond the default licence scope. The restriction on forwarding to competing pentest firms (9.3) is narrow by design, but clients with panel arrangements may want it removed entirely.
- _Liability caps._ Enterprise and public sector procurement will often seek higher caps for data protection or confidentiality breaches (a "super cap"), or unlimited liability for certain categories. The templates do not include a super cap; if your insurance and risk appetite support one, feel free to add one.
- _Audit evidence (DPA 7.2)._ The DPA offers flexible audit evidence options. Clients with specific regulatory requirements (FCA-regulated firms, for example) may require particular certifications or on-site audit rights beyond the defaults.
- _Marketing and client naming (MSA 10.7)._ The default requires prior written consent. Some clients will want explicit contractual prohibition, others will be happy to give it. You know your clients best!

## Updates and support

These templates are maintained as regulation changes. Watch this repo for release notifications.

Please join us on [Slack](https://pwnlegal.slack.com) to discuss and provide feedback on the templates!

For bespoke drafting, regulatory advice, or retainer arrangements: [rich@pwn.legal](mailto:rich@pwn.legal)

## Licence

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Adapt freely with attribution to [pwn.legal](https://pwn.legal).

## Disclaimer

Nothing in this repo constitutes legal advice. Please adapt these templates to your circumstances with the benefit of independent legal advice.

Enjoy!
