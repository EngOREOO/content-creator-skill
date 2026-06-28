# Arabic Content Quality Scoring Engine

**0–100 Comprehensive Evaluation Rubric for Arabic Marketing & Business Content**

Based on analysis of 234 Middle Eastern tech company websites across 7 countries, Saudi localization patterns, negative pattern blacklists, and style guide best practices.

---

## Scoring Overview

| Category | Max Points | Weight |
|----------|-----------|--------|
| 1. Naturalness | 20 | 20% |
| 2. Saudi Localization | 20 | 20% |
| 3. Persuasiveness | 15 | 15% |
| 4. SEO Quality | 10 | 10% |
| 5. Authority & Trust | 10 | 10% |
| 6. Clarity | 10 | 10% |
| 7. Readability | 5 | 5% |
| 8. Conversion Potential | 5 | 5% |
| 9. Originality | 5 | 5% |
| **TOTAL** | **100** | **100%** |

**Pass threshold:** 75/100 (scores below trigger mandatory rewrite)
**Excellent:** 90–100
**Good:** 75–89
**Needs rewrite:** 50–74
**Reject:** 0–49

---

## 1. Naturalness (0–20 points)

### Description
Measures whether the content reads as if a native Arabic speaker wrote it. The primary differentiator between human-quality Arabic content and machine-translated or non-native writing. This is the highest-weighted category because unnatural Arabic undermines all other quality dimensions — a Saudi reader who detects translation artifacts will distrust the entire piece.

### What to Look For
- Fluent Modern Standard Arabic (MSA) sentence flow
- Natural word choices that a Saudi marketing professional would use
- Absence of English sentence structures mirrored in Arabic
- Proper use of Arabic connectors (و، ف، لكن) rather than English-style connectors
- Varied sentence openings (not starting every sentence with "نحن" or "إن")
- Arabic-specific rhythm and cadence appropriate to business context
- Idiomatic expressions used correctly and sparingly
- Appropriate level of formality for the context

### What to Deduct For
- **Translation artifacts (–4 to –8):** Word-for-word English-to-Arabic translations. Signatures: long定语 chains, English sentence structure, unnatural preposition use
- **GPT/AI markers (–3 to –6):** Sentences starting with "بالتأكيد،" "فعلاً،" "من الجدير بالذكر" at the start of paragraphs. Overuse of "جداً" as intensifier
- **Overuse of "حلول" (–1 to –3):** Using "حلول" (solutions) in every sentence as a direct carryover from English
- **Wrong register (–2 to –4):** Using classical Arabic (فصحى معقدة) where simple MSA is appropriate, or dialect where فصحى is expected
- **Literal idiom translation (–3):** English idioms translated word-for-word (e.g., "يكسر الجليد" for "break the ice")
- **Gender agreement errors (–2 to –5):** Inconsistent grammatical gender for technical terms ("المنصة الجديد" instead of "المنصة الجديدة")
- **"رجاءً" overuse (–1 to –2):** Using "رجاءً" in CTAs instead of direct imperative
- **Code-switching errors (–1 to –3):** More than 2–3 English terms per Arabic sentence; Arabic suffixes on English words ("API-اتنا")

### Scoring Rubric

| Score | Level | Description | Example Characteristics |
|-------|-------|-------------|----------------------|
| 18–20 | Native | Reads like it was written by a Saudi marketing professional for a Saudi audience | Varied sentence structure, natural connectors, appropriate MSA, zero translation artifacts, English terms used only where natural |
| 14–17 | Near-native | Minor non-native tells but overall fluent | Occasional English sentence structure mirrored, one or two awkward word choices, but reads naturally overall |
| 8–13 | Translationese | Clearly translated or written by non-native speaker | Multiple translation artifacts, repetitive sentence openings, overuse of "نحن" and "إن", several GPT markers |
| 4–7 | Machine-sounding | Reads like raw MT output | Word-for-word translation, wrong prepositions, unnatural word order, multiple gender errors |
| 0–3 | Unusable | Gibberish or incomprehensible Arabic | Severe grammar errors, completely wrong register, content that a native reader would not understand |

### Example Scoring

**Sample A (18/20):**
> نوفر للبنوك السعودية حلولاً لأتمتة الامتثال التنظيمي. نستخدم الذكاء الاصطناعي لتحليل المعاملات آنياً وتقليل وقت المراجعة اليدوية بنسبة ٨٥٪.
> *Natural MSA, appropriate technical terms, specific numbers, no translation artifacts, natural rhythm.*

**Sample B (10/20):**
> بالتأكيد، نحن نقدم حلولاً متطورة جداً في عالم التكنولوجيا. حلولنا المبتكرة والمتميزة تساعد الشركات على تحقيق أهدافها من خلال الاستفادة من أحدث ما توصلت إليه التكنولوجيا في الذكاء الاصطناعي.
> *GPT markers ("بالتأكيد"), overuse of "حلول", empty adjectives, "أحدث ما توصلت إليه التكنولوجيا" cliché, repetitive structure.*

### Edge Cases
- **Code-switching in technical content:** A developer-facing page may naturally use more English terms. Score based on the intended audience — if the code-switching matches the audience expectation, reduce the deduction.
- **Intentional dialect in social media:** If the content is for TikTok/Instagram and uses deliberate Saudi dialect for cultural resonance, do not penalize as long as it is consistent and intentional.
- **Brand-specific voice:** Some brands deliberately use a more formal or more casual voice. Score against the brand's own style guide, not against a universal standard.

---

## 2. Saudi Localization (0–20 points)

### Description
Measures how well the content adapts to the Saudi Arabian market specifically. Content that works for UAE, Egypt, or the broader MENA region may fail here. Saudi audiences have distinct expectations around formality, national pride, Vision 2030 alignment, and business vocabulary. This is weighted equally with Naturalness because Saudi localization errors immediately signal that the content was not written for Saudi readers.

### What to Look For
- Correct Saudi business terminology (التحول الرقمي, تمكين, حوكمة, توطين)
- Vision 2030 alignment phrased correctly ("تماشياً مع رؤية المملكة ٢٠٣٠")
- Saudi government entity references (SDAIA, CST, ZATCA, DGA) used accurately
- Appropriate formality level (more formal than UAE, less formal than government circulars)
- Saudi-specific trust signals (PIF, ministry clients, Saudi leadership bios)
- Saudi business culture awareness (relationship-first, proper greetings)
- Use of Saudi-appropriate verb forms (نقدم, نعمل — never بنقدم, منقدم)
- Saudi numerals (1, 2, 3 preferred over ١, ٢, ٣ in most business contexts)
- Hijri dates alongside Gregorian where appropriate

### What to Deduct For
- **UAE/Egyptian content reused for Saudi (–5 to –10):** Copy-pasted content that references Dubai instead of Riyadh, uses Emirati terminology, or lacks Saudi context
- **Egyptian dialect words (–3 to –8):** "بنقدم" instead of "نقدم", "عندنا" instead of "لدينا", "دلوقتي" instead of "حالياً"
- **Missing Vision 2030 alignment (–2 to –5):** Saudi-targeted content that ignores the national transformation context
- **Wrong government references (–3 to –6):** Referencing the wrong regulatory body, using outdated ministry names, or misstating Vision 2030 language
- **Overly classical Arabic (–2 to –4):** "إنَّ" emphasis particles, "لقد" constructions, classical verb forms that sound unnatural in Saudi business
- **Casual CTAs (–1 to –3):** "كلمنا" instead of "تواصل معنا", "ابعتلنا" instead of "أرسل لنا"
- **Missing Saudi trust signals (–2 to –5):** Content targeting Saudi enterprises without any Saudi client references, Saudi certifications, or Saudi partnership mentions
- **Incorrect formality level (–1 to –3):** Too informal for government-adjacent content, or too stiff for B2C tech

### Scoring Rubric

| Score | Level | Description |
|-------|-------|-------------|
| 18–20 | Native Saudi | Could only have been written for Saudi Arabia. Correct terminology, natural Vision 2030 integration, appropriate formality, Saudi-specific trust signals throughout |
| 14–17 | Saudi-adapted | Clearly written for Saudi market with minor missed opportunities. Mostly correct terminology, one or two non-Saudi phrases |
| 8–13 | Generic Arabic | Reads like generic Arabic content that could be for any Arab country. No Saudi-specific localization beyond changing the country name |
| 4–7 | Wrong market | Uses terminology from another Arab market (Egyptian, Levantine, or Emirati patterns dominate). Saudi readers would sense it wasn't written for them |
| 0–3 | Unlocalized | English content machine-translated to Arabic with zero Saudi market awareness. No Saudi terminology, wrong formality level |

### Example Scoring

**Sample A (19/20):**
> شريكك الموثوق في التحول الرقمي — تماشياً مع رؤية المملكة ٢٠٣٠. نعمل مع أكثر من ١٠ جهات حكومية سعودية، ومعتمدون من هيئة الحكومة الرقمية.
> *Correct Saudi formula ("شريكك الموثوق في"), Vision 2030 reference, Saudi government client reference, DGA certification, Saudi business formality level.*

**Sample B (7/20):**
> احنا شركة برمجة بنقدم حلول تكنولوجيا معلومات متطورة. عندنا خبرة كبيرة في السوق. فريقنا شغوف بالابتكار.
> *Egyptian dialect ("احنا", "بنقدم"), vague claims, "شغوف" cliché, no Saudi market awareness, wrong formality register.*

### Edge Cases
- **International brands in Saudi:** A global brand may deliberately use less Saudi-specific language. Score against the brand's positioning — if they position as global, Saudi localization should still be present but may be lighter.
- **Technical vs. marketing content:** API documentation requires less localization than homepage copy. Adjust expectations proportionally.
- **Multilingual sites:** Saudi sites that use English as primary language still need localization cues (Saudi case studies, local certifications, Vision 2030 references in English).

---

## 3. Persuasiveness (0–15 points)

### Description
Measures the content's ability to convince a Saudi reader to take the desired action. Persuasion in the Saudi market differs from Western markets — it relies more on trust, national alignment, relationship signals, and logical argumentation than on aggressive sales tactics or emotional hype.

### What to Look For
- Clear value proposition stated within the first 2 sentences
- Problem → Solution → Benefit → CTA structure
- Emotional resonance with Saudi audience (national pride, trust, family, stability, growth)
- Logical argument structure with specific evidence
- Objection handling (addressing common Saudi buyer concerns: security, compliance, reliability, local support)
- Credibility building through specific proof points
- Social proof appropriate to Saudi context (government clients, local partnerships)
- Risk reversal where applicable (free consultation, trial, Saudi-based support)

### What to Deduct For
- **No clear value prop (–3 to –5):** Reader finishes the first paragraph unable to state what the company offers
- **Vague claims without evidence (–2 to –4):** "نحن الأفضل" without data, "حلول متطورة" without specifics
- **Wrong persuasion approach (–2 to –4):** Aggressive US-style sales language that feels pushy to Saudi readers, or excessive humility that undermines credibility
- **Missing social proof (–1 to –3):** Claims without client names, numbers, or recognizable references
- **No objection handling (–1 to –2):** Ignoring common Saudi objections about security, local support, or compliance
- **Weak argument structure (–2 to –3):** Rambling paragraphs that don't build a coherent case
- **No clear CTA (–1 to –2):** Reader finishes unsure what to do next

### Scoring Rubric

| Score | Level | Description |
|-------|-------|-------------|
| 13–15 | Highly persuasive | Clear value prop in first sentence, logical argument with evidence, emotional resonance with Saudi audience, handles objections naturally, compelling CTA |
| 10–12 | Persuasive | Good value prop, reasonable argument structure, some evidence, adequate CTA. Would convince a moderately interested buyer |
| 7–9 | Moderate | Value prop exists but buried, argument is present but weak, limited evidence, CTA is generic. May not convince skeptical readers |
| 4–6 | Weak | Unclear value, no argument structure, generic claims, no evidence, weak or missing CTA |
| 0–3 | Not persuasive | No value proposition, random claims, reader learns nothing about why they should care |

### Example Scoring

**Sample A (14/15):**
> ٧٣٪ من الشركات السعودية تستخدم أنظمة إدارة قديمة تخسرها ٤٠٠ ساعة عمل سنوياً. منصتنا تؤتمت هذه العمليات في ٣ أيام — لا تغيير في البنية التحتية الحالية. اختبرت مع ٣ بنوك سعودية. احجز عرضاً تجريبياً مجاناً.
> *Problem → statistic → solution → objection handling (no infrastructure change) → proof → compelling CTA.*

**Sample B (5/15):**
> نحن شركة رائدة في مجال التقنية. نقدم حلولاً مبتكرة. فريقنا محترف. خدماتنا متميزة. تواصل معنا.
> *No value proposition, no evidence, no structure, generic claims, weak CTA.*

### Edge Cases
- **Direct vs. indirect persuasion:** Saudi B2B content often uses more direct persuasion than Western B2B (naming specific prices, competitors, or results). Do not penalize directness.
- **Relationship-first content:** Some Saudi content invests heavily in relationship-building before a direct pitch. This is culturally appropriate but must still provide value in the relationship-building phase.

---

## 4. SEO Quality (0–10 points)

### Description
Measures the content's search engine optimization for Arabic-language queries. Arabic SEO differs from English SEO in keyword structure, search intent patterns, meta description conventions, and schema requirements.

### What to Look For
- Arabic keyword optimization (primary keyword in H1, first 100 words, meta description)
- Meta description: 150–160 characters, keyword in first 60 chars, includes value prop + CTA
- Heading hierarchy (H1 → H2 → H3, no skipped levels)
- Content depth sufficient for the topic (not thin content)
- Arabic search intent matching (هل/كيف/ما هي patterns for informational queries)
- Arabic schema markup (inLanguage: ar, Organization schema with Arabic name)
- URL structure using English transliteration of Arabic keywords
- Question-form H2s for informational content ("هل تبحث عن أفضل شركة برمجة؟")
- Internal linking using Arabic anchor text

### What to Deduct For
- **No keyword targeting (–1 to –3):** Content written without any consideration for what users search for in Arabic
- **Keyword stuffing (–2 to –3):** Unnatural repetition of the same Arabic keyword phrase, especially in headings
- **Missing or weak meta description (–1 to –2):** No meta description, or one that doesn't include the target keyword or compelling CTA
- **Poor heading structure (–1 to –2):** No H1, multiple H1s, skipped heading levels, headings that don't contain keywords
- **Thin content (–1 to –3):** Less than 300 words for a topic that requires depth, or content that doesn't cover the topic comprehensively
- **Wrong search intent (–1 to –2):** Writing transactional content when searchers want informational content (or vice versa)
- **Arabic URLs (–1):** Arabic characters in URL instead of transliterated English slugs
- **No schema (–1):** Missing Organization, Article, or FAQ schema for Arabic pages

### Scoring Rubric

| Score | Level | Description |
|-------|-------|-------------|
| 9–10 | Excellent | Proper keyword targeting, excellent meta, strong heading hierarchy, appropriate depth, correct intent, Arabic schema |
| 7–8 | Good | Most SEO elements present, minor gaps (e.g., meta is good but schema missing) |
| 5–6 | Average | Basic keyword use, acceptable headings, but thin content or weak meta |
| 3–4 | Below average | Multiple SEO gaps — no meta, poor headings, no keyword strategy |
| 0–2 | Poor | No SEO consideration whatsoever |

### Example Scoring

**Sample A (9/10):**
> H1: "شركة برمجة في الرياض — حلول تقنية مخصصة"
> Meta: "شركة برمجة في الرياض — نقدم حلول تقنية مخصصة للشركات. ٥٠٠+ مشروع في ١٠ سنوات. احصل على استشارة مجانية."
> Structure: H1 → H2 (خدماتنا, لماذا نحن؟, عملاؤنا) → H3 within services.
> *Keyword in H1 and meta, good length, logical structure, Arabic schema available.*

**Sample B (3/10):**
> H1: "مرحباً بكم"
> Meta: none
> Structure: no H2s, single paragraph of 800 words
> *No keyword targeting, no meta, no structure, no SEO consideration.*

### Edge Cases
- **Brand searches vs. generic keywords:** Established brands may optimize for brand + service rather than generic keywords. Score against the actual search strategy.
- **Voice search optimization:** Increasingly important for Arabic SEO. Content that answers "كيف" and "ما هي" questions scores higher.

---

## 5. Authority & Trust (0–10 points)

### Description
Measures how effectively the content builds credibility and trust with the Saudi audience. Saudi readers are among the most trust-signal-sensitive in the world — analysis of 234 sites showed Saudi companies average 6.2 trust signals per page, 3–7 times more than US/European equivalents.

### What to Look For
- Trust signals placed prominently (above the fold, near CTAs)
- Specific evidence and proof points (numbers, statistics, named clients)
- Expertise demonstration (years in market, team credentials, thought leadership)
- Partnership/certification references (Saudi-specific: SDAIA, CST, ZATCA, DGA plus global: ISO, Microsoft Gold, AWS)
- Testimonial quality (full attribution: name, title, company, photo)
- Case study availability and depth
- Client logo display with recognizable Saudi names
- Awards and recognition relevant to Saudi market

### What to Deduct For
- **No trust signals (–2 to –5):** Content that makes claims without any credibility support
- **Generic trust claims (–1 to –3):** "نحن موثوقون" without evidence, "عملاؤنا سعداء" without testimonial specifics
- **Fake or exaggerated claims (–3 to –5):** Numbers that seem fabricated, "أكثر من ١٠٠٠ عميل" for a startup, unverifiable "first in the world" claims
- **Missing Saudi-specific certification (–1 to –3):** Targeting Saudi enterprises without mentioning CST, NCA, SDAIA, or ZATCA compliance
- **Stock testimonials (–1 to –2):** "قال العميل: خدمة ممتازة" without name, title, or company — these reduce trust rather than building it
- **No social proof (–1 to –2):** No client logos, no partner mentions, no case study references
- **Overwhelming trust signals (–1):** More than 12 logos in a grid without grouping or context

### Scoring Rubric

| Score | Level | Description |
|-------|-------|-------------|
| 9–10 | High authority | Multiple specific trust signals with evidence, Saudi certifications, named clients, full-attribution testimonials, case studies |
| 7–8 | Good authority | Several trust signals, some specificity, at least one Saudi-specific certification or client name |
| 5–6 | Moderate | Basic trust signals (client count, years), but no specifics or Saudi-specific references |
| 3–4 | Low | Few trust signals, generic claims, no verifiable evidence |
| 0–2 | No trust | Claims without any support, no certifications, no testimonials, no evidence |

### Example Scoring

**Sample A (10/10):**
> نخدم أكثر من ٢٠٠ عميل في المملكة، منهم ٣ جهات حكومية و ١٢ شركة مدرجة. معتمدون من هيئة الحكومة الرقمية و ISO 27001. — "ساعدونا في تقليل وقت المعالجة بنسبة ٧٠٪" — محمد الغامدي، مدير تقنية المعلومات، شركة الاتصالات السعودية.
> *Specific numbers, named government clients, Saudi certification, full-attribution testimonial.*

**Sample B (3/10):**
> نحن شركة موثوقة ذات خبرة طويلة. عملاؤنا يحبون خدماتنا. فريقنا محترف.
> *No specific trust signals, no evidence, no named clients, no certifications, generic testimonials.*

### Edge Cases
- **Startups:** New companies may lack extensive client lists or certifications. Score based on what they can demonstrate (team expertise, founder credentials, pilot clients, partnership in progress).
- **Enterprise vs. SMB:** Enterprise content needs more and higher-level trust signals. SMB content can rely on user count and social proof.

---

## 6. Clarity (0–10 points)

### Description
Measures how easily a Saudi reader understands the content on first reading. Arabic business content suffers from a common pattern of overly complex sentence structures, unnecessary connectors, and buried meaning.

### What to Look For
- Message clarity: Can the reader state what the company does after one read?
- Sentence structure: Varied but not convoluted; subject-verb-object preferred
- Logical flow: Information progresses naturally (Problem → Solution → Benefit → CTA)
- Jargon management: Technical terms explained when necessary, not assumed
- Arabic readability: Appropriate for business audience (Grade 6–8 equivalent)
- One topic per paragraph
- Active voice predominates
- Transition words used appropriately, not excessively

### What to Deduct For
- **Buried message (–2 to –4):** Reader cannot determine what the company offers within the first paragraph
- **Convoluted sentences (–1 to –3):** Chains of "حيث" and "والتي" that create run-on sentences
- **Overuse of filler phrases (–1 to –3):** "مما لا شك فيه", "في عالمنا المعاصر", "من هنا كان لا بد من" — phrases that add nothing
- **Jargon without explanation (–1 to –2):** Heavy technical terminology without context for business readers
- **Passive voice overuse (–1):** "يتم تقديم الحلول" instead of "نقدم الحلول"
- **No logical structure (–2 to –4):** Random ordering of information, topics jumping between paragraphs
- **Missing topic sentences (–1):** Paragraphs that start without indicating what they cover

### Scoring Rubric

| Score | Level | Description |
|-------|-------|-------------|
| 9–10 | Crystal clear | Instant understanding, perfect logical flow, appropriate simplicity without being simplistic |
| 7–8 | Clear | Easy to understand, minor areas of confusion, generally good structure |
| 5–6 | Adequate | Understandable but requires re-reading some parts, occasional rambling |
| 3–4 | Confusing | Hard to follow, multiple re-reads needed, buried message, poor structure |
| 0–2 | Incomprehensible | Cannot determine what the content is about after multiple reads |

### Example Scoring

**Sample A (9/10):**
> تواجه شركات التجزئة في السعودية تحدياً في إدارة المخزون. ٤٠٪ من المخزون يهدر سنوياً بسبب عدم الدقة. نظامنا يتنبأ بالطلب بدقة ٩٥٪. يقلص الهدر بنسبة ٦٠٪ في أول ٣ أشهر. احجز عرضاً تجريبياً.
> *Clear problem, specific data, direct solution, measurable benefit, clear CTA. One idea per sentence.*

**Sample B (4/10):**
> مما لا شك فيه أن في عالمنا المعاصر المتسارع والمتغير، حيث التكنولوجيا تلعب دوراً محورياً في شتى المجالات، أصبح من الضروري على المؤسسات والشركات على حد سواء سواء كانت كبيرة أو صغيرة مواكبة هذا التطور من خلال الاستفادة من الحلول التقنية المتطورة والتي تعمل على تحسين الأداء ورفع الكفاءة وذلك من خلال...
> *Filler opening, no topic sentence, run-on with "حيث" and "والتي", message is unclear, no structure.*

### Edge Cases
- **Complex topics:** AI, blockchain, and deep tech content requires some complexity. Score on whether the complexity is well-structured, not on whether it's simple.
- **Legal/compliance content:** Naturally more complex. Judge against legal writing standards, not marketing standards.

---

## 7. Readability (0–5 points)

### Description
Measures the visual and structural readability of the Arabic content. Arabic has specific readability requirements that differ from English — longer line heights, RTL formatting considerations, different paragraph density expectations.

### What to Look For
- Sentence length appropriate for Arabic business content (hero: 5–10 words, body: 8–15 words)
- Paragraph structure: 2–4 sentences for body content, 1–2 for hero sections
- Visual formatting: bullets, bold for key points, adequate white space
- Mobile readability: short paragraphs, scannable content
- RTL formatting quality: proper alignment, no LTR artifacts in Arabic text
- Bold used for key numbers and benefits (1 per paragraph max)
- Heading hierarchy visually apparent
- Bullet points with parallel structure

### What to Deduct For
- **Wall of text (–1 to –2):** Paragraphs longer than 5 sentences without breaks
- **Run-on sentences (–1):** Arabic sentences exceeding 20 words without punctuation
- **Poor formatting (–1):** No bold, no bullets, no visual hierarchy
- **RTL issues (–1 to –2):** English punctuation in Arabic text, mixed comma styles, misaligned text
- **Too many bullets (–1):** Lists exceeding 6 items without grouping
- **Inconsistent bullet structure (–1):** Mixing verb-starting and noun-starting bullets

### Scoring Rubric

| Score | Level | Description |
|-------|-------|-------------|
| 5 | Excellent | Perfect readability for Arabic web. Short sentences, well-structured paragraphs, good visual hierarchy, RTL correct |
| 4 | Good | Mostly readable, minor formatting issues or one long paragraph |
| 3 | Adequate | Readable but could be improved — some long paragraphs, inconsistent formatting |
| 2 | Below average | Dense text, poor formatting, readability issues that affect comprehension |
| 0–1 | Poor | Wall of text, no structure, RTL issues make reading difficult |

### Example Scoring

**Sample A (5/5):**
> نقدم حلول الذكاء الاصطناعي للقطاع المالي. (8 words)
> خبرتنا تمتد لأكثر من ١٠ سنوات مع ٥ بنوك رئيسية. (9 words)
> ساعدنا بنك الرياض في تقليل وقت المعالجة بنسبة ٧٠٪. (8 words)
> **تواصل معنا** لمناقشة احتياجاتك. (5 words)
> *Short sentences, single-idea paragraphs, bold CTA, good rhythm.*

**Sample B (1/5):**
> في ظل التطورات المتسارعة في عالم التكنولوجيا والتحول الرقمي الذي تشهده المملكة العربية السعودية في ظل رؤية ٢٠٣٠ حيث أصبحت الحلول التقنية ضرورة ملحة ولا غنى عنها للمؤسسات والشركات سواء كانت صغيرة أو كبيرة فإننا في شركتنا نسعد بتقديم حلولنا المتطورة والمبتكرة والتي تعمل على تحقيق أهداف عملائنا من خلال الاستفادة من أحدث التقنيات...
> *Single run-on paragraph with no breaks, no visual hierarchy, no bold, no structure.*

### Edge Cases
- **Long-form content:** Whitepapers and guides may have longer paragraphs. Acceptable if varied with subheadings, pull quotes, and visual breaks.

---

## 8. Conversion Potential (0–5 points)

### Description
Measures the content's ability to drive the reader to take the desired action. Saudi conversion patterns differ from Western markets — urgency must be balanced with relationship-building, and CTAs must be value-forward rather than pushy.

### What to Look For
- CTA quality: specific, benefit-oriented, action-driven (not "اضغط هنا" or "اعرف المزيد")
- Urgency/action triggers appropriate for Saudi market (time-limited offers, limited availability, but not aggressive pressure)
- Friction reduction: addressing objections before the CTA, offering risk reversal
- Value clarity: reader knows what they get by taking action
- Trust sufficiency for action: enough trust signals near the CTA to overcome hesitation
- CTA placement: hero, mid-content, and end-of-content minimum
- CTA language: direct but respectful, formal imperative form

### What to Deduct For
- **Weak CTAs (–1 to –2):** "اضغط هنا", "اعرف المزيد", "تواصل معنا" as primary CTA without context
- **No CTA (–2):** Content that ends without telling the reader what to do
- **Too many CTAs (–1):** More than 6 CTAs per page creating choice paralysis
- **High-friction CTA (–1):** "احصل على عرض سعر" before value is proven, long forms without incentive
- **No risk reversal (–1):** Nothing that reduces the perceived risk of taking action
- **Missing value context (–1):** CTA that doesn't state what happens after clicking
- **Wrong CTA tone (–1):** Too casual ("كلمنا") or too aggressive ("اشترك الآن أو سترتفع الأسعار")

### Scoring Rubric

| Score | Level | Description |
|-------|-------|-------------|
| 5 | High conversion | Compelling, specific CTAs with clear value, placed at decision points, low friction, risk reversal |
| 4 | Good | Effective CTAs, minor improvements possible (more specificity, better placement) |
| 3 | Adequate | CTAs present but generic, acceptable placement |
| 2 | Below average | Weak CTAs, poor placement, missing key conversion elements |
| 0–1 | Poor | No or terrible CTAs, high friction, reader doesn't know what to do |

### Example Scoring

**Sample A (5/5):**
> احجز استشارة مجانية مدتها ٣٠ دقيقة مع خبير تقني — لا توجد التزامات.
> *Specific, free (risk reversal), low-friction ("لا توجد التزامات"), names the value.*

**Sample B (1/5):**
> اضغط هنا
> *Laziest possible CTA, no value, no context, no urgency.*

### Edge Cases
- **Brand awareness content:** Blog posts or thought leadership may have softer CTAs (اشترك في النشرة البريدية). Score against the content's actual conversion goal.
- **Multi-step conversion:** Some Saudi B2B sales cycles require multiple touches. A single piece may only aim for the next step (تنزيل الدراسة), not the final sale.

---

## 9. Originality (0–5 points)

### Description
Measures how differentiated the content is from competitors and how creatively it approaches the topic. Arabic tech content suffers from extreme homogeneity — most companies use the same phrases, structures, and approaches.

### What to Look For
- Differentiation from competitors: Does it say something unique, or is it interchangeable?
- Unique angle: A fresh take on the topic, not the standard industry boilerplate
- Avoidance of clichés: None of the banned phrases from the negative patterns list
- Fresh perspective: New insights, data, or arguments, not rehashed common knowledge
- Creative approach to structure, examples, or framing
- Specificity that only this company could write

### What to Deduct For
- **Cliché overload (–1 to –3):** Multiple banned phrases from the negative patterns list (ثورة, يغير قواعد اللعبة, حل شامل, etc.)
- **Template content (–1 to –2):** Reads like a generic industry template that any competitor could publish
- **No differentiation (–1 to –2):** Content that doesn't distinguish the company from competitors in any way
- **Rehashed content (–1):** Arguments and examples that appear on every competitor's site
- **Copycat structure (–1):** Following the exact same heading structure as competitors without adding unique value

### Scoring Rubric

| Score | Level | Description |
|-------|-------|-------------|
| 5 | Highly original | Unique angle, zero clichés, specific insights only this company could provide, creative structure |
| 4 | Original | Mostly fresh content, minor clichés, some differentiation |
| 3 | Adequate | Mix of original and templated content, some differentiation attempts |
| 2 | Below average | Mostly templated, heavy cliché use, little differentiation |
| 0–1 | Unoriginal | Complete template content, indistinguishable from competitors, cliché-heavy |

### Example Scoring

**Sample A (5/5):**
> بينما تركز شركات التقنية على سرعة المعالجة، ركزنا على شيء آخر: دقة القرار. نظامنا يقلص速度快 بنسبة ٢٠٪ فقط — لكنه يزيد دقة القرارات بنسبة ٣٤٠٪. لأن speed without accuracy هو مجرد أخطاء أسرع.
> *Unique angle (accuracy over speed), specific data, differentiated positioning, creative framing.*

**Sample B (1/5):**
> نحن شركة رائدة في تقديم الحلول التقنية المبتكرة. نستخدم أحدث ما توصلت إليه التكنولوجيا. حلولنا تغير قواعد اللعبة. معاً نحو مستقبل رقمي أفضل.
> *Every sentence is a cliché. Could be any tech company. Zero differentiation.*

### Edge Cases
- **Evergreen content:** Some topics (e.g., "ما هو التحول الرقمي") are inherently less differentiated. Score on execution quality and unique examples within the constrained topic.

---

## Automatic Rewrite Triggers

The following conditions trigger an automatic rewrite of the content regardless of overall score. Any one trigger is sufficient to reject the content in its current form.

### Trigger 1: Any Forbidden Phrase
**Condition:** Content contains one or more phrases from the hard blacklist.
**Action:** Immediate rewrite required. Score is irrelevant.
**Blacklist includes:**
- ثورة في عالم / ثورة في مجال
- يُغير قواعد اللعبة / game-changing
- أحدث ما توصلت إليه التكنولوجيا / cutting-edge
- المستقبل هنا / the future is here
- نحن شغوفون / we are passionate
- تحت الغطاء / تحت الكابوت / under the hood
- مما لا شك فيه / لا شك أن
- في عالمنا المعاصر / في عالمنا اليوم
- نحو مستقبل أفضل / نحو غدٍ مشرق
- بكل سهولة ويسر / بسهولة تامة
- تجدر الإشارة إلى / من الجدير بالذكر
**Rationale:** These phrases are so overused or signal low quality so strongly that they poison any content they appear in.

### Trigger 2: Score Below 75
**Condition:** Overall weighted score is below 75/100.
**Action:** Rewrite required. Content that scores below 75 has fundamental issues in naturalness, localization, or clarity that cannot be fixed with minor edits.
**Note:** Scores between 50–74 may be salvageable with targeted rewrites. Scores below 50 indicate a complete rewrite from scratch.

### Trigger 3: Detected Machine Translation
**Condition:** Clear evidence that the content was machine-translated from English to Arabic without human editing.
**Detection markers:**
- Word-for-word English sentence structure mirrored in Arabic
- Repeated "بالتأكيد" at sentence starts >3 times per page
- Multiple gender agreement errors
- Literal translations of English idioms
- "رجاءً" used in contexts where Arabic uses direct imperative
- "حلول" appears in >30% of sentences
- Impossibly long sentences (>30 words) with comma splicing
**Action:** Rewrite by a native Arabic copywriter. Machine translation can be used as a starting draft but must be fully rewritten by a human.

### Trigger 4: Missing Saudi Localization in Saudi-Targeted Content
**Condition:** Content explicitly or implicitly targets Saudi Arabia (Saudi client references, Saudi pricing, Saudi contact info) but does not include appropriate Saudi localization.
**Detection markers:**
- Uses Egyptian dialect verbs (بنقدم, عندنا) in Saudi-targeted content
- No Vision 2030 reference in content that discusses national transformation
- References UAE/Dubai as the primary market context
- No Saudi-specific certifications or regulatory references
- Wrong formality level for Saudi business context
**Action:** Localize for Saudi market. Minimum: correct MSA verb forms, Vision 2030 alignment, Saudi-specific terminology, appropriate formality level.

### Trigger 5: Plagiarism Detection
**Condition:** Content matches existing published content beyond acceptable threshold.
**Detection:**
- >30% direct match with any single source
- >15% match with competitor content
- Entire paragraphs copied from another source
- Same unique phrasing as another company's content
**Action:** Complete rewrite. Plagiarized content damages SEO, brand credibility, and legal standing.

### Trigger 6: Inappropriate Tone
**Condition:** Tone is fundamentally wrong for the target audience and context.
**Detection markers:**
- Overly casual for government/enterprise content ("يلا", "تمام", "ماشي")
- Overly aggressive for Saudi business culture (threatening urgency, pressure tactics)
- Overly academic for web content (heavy classical Arabic, complex grammatical structures)
- Sarcastic or humorous tone in formal business context
- Patronizing or condescending language
**Action:** Rewrite to match the appropriate tone for the audience and channel.

### Trigger 7: Missing or Broken Structure
**Condition:** Content lacks basic structural elements needed for web readability.
**Detection:**
- No heading hierarchy (no H1, no H2 breaks)
- Single paragraph longer than 300 words
- No paragraph breaks for more than 500 words
- No clear section differentiation
**Action:** Restructure content with proper heading hierarchy, paragraph breaks, and visual formatting.

---

## Complete Scoring Examples

### Example 1: Tech Startup Homepage — "منصة ذكاء"

**Text:**
> منصة ذكاء — حل ذكي لإدارة علاقات العملاء. فريقنا شغوف بتقديم أفضل الحلول. نغير قواعد اللعبة في عالم CRM. مستقبل المبيعات هنا. حلولنا المبتكرة والمتطورة تساعد الشركات على النمو. بكل سهولة ويسر، يمكنك إدارة جميع عمليات البيع. سجل الآن وابدأ رحلتك نحو النجاح.

| Category | Score | Max | Rationale |
|----------|-------|-----|-----------|
| Naturalness | 4 | 20 | Multiple clichés, "شغوف", "يغير قواعد اللعبة", "المستقبل هنا", "بكل سهولة ويسر", "حلول" in nearly every sentence. Reads as low-quality MT or template content |
| Saudi Localization | 3 | 20 | Zero Saudi localization. No Vision 2030, no Saudi terminology, generic Arabic. "سجل الآن" is a weak CTA for Saudi market |
| Persuasiveness | 2 | 15 | No value proposition. No evidence. No problem statement. Just empty claims. Reader has no reason to act |
| SEO Quality | 3 | 10 | "حل ذكي" is a generic keyword. No meta structure evident. Thin content |
| Authority & Trust | 0 | 10 | Zero trust signals. No numbers, clients, certifications, or testimonials |
| Clarity | 3 | 10 | Buried message. Unclear what the platform actually does. "إدارة علاقات العملاء" is buried in the first sentence |
| Readability | 2 | 5 | Wall of marketing claims. No visual structure. Run-on feel |
| Conversion Potential | 1 | 5 | "سجل الآن" — worst CTA. No value. No risk reversal. High friction |
| Originality | 0 | 5 | Zero originality. Every sentence is a known cliché from the blacklist |
| **TOTAL** | **18** | **100** | **REJECT — Multiple automatic rewrite triggers triggered** |

**Rewrite triggers hit:**
- ✅ Forbidden phrases: "شغوف", "يغير قواعد اللعبة", "المستقبل هنا", "بكل سهولة ويسر"
- ✅ Score below 75 (18/100)
- ✅ Inappropriate tone (cliché-heavy, no substance)
- ✅ Missing Saudi localization
- ✅ Missing structure

---

### Example 2: Mid-Sized Saudi Tech Company — "تقنية التميز"

**Text:**
> شريكك الموثوق في التحول الرقمي. نعمل تماشياً مع رؤية المملكة ٢٠٣٠ لتمكين المؤسسات من تحقيق التميز التشغيلي. خبرتنا تمتد لأكثر من ١٥ عاماً في السوق السعودي مع أكثر من ٢٠٠ عميل. منصتنا تستخدم الذكاء الاصطناعي لتحليل بيانات العملاء وتقديم توصيات دقيقة. وفرنا لعملائنا متوسط ٣٥٪ من تكاليف التشغيل في السنة الأولى. معتمدون من هيئة الحكومة الرقمية. احجز استشارة مجانية — ٣٠ دقيقة مع خبير تقني.
>
> نقدم حلولاً في:
> • إدارة علاقات العملاء (CRM)
> • أتمتة المبيعات والتسويق
> • تحليلات الأعمال المتقدمة
> • تكامل الأنظمة المؤسسية
>
> قال عبدالله السبيعي، مدير تقنية المعلومات في إحدى شركات الاتصالات: «خفضنا وقت معالجة التذاكر بنسبة ٧٠٪ في أول شهرين».

| Category | Score | Max | Rationale |
|----------|-------|-----|-----------|
| Naturalness | 16 | 20 | Natural MSA. Appropriate use of English tech terms. One slight awkwardness: "وفرنا لعملائنا متوسط" could be smoother. But overall native quality |
| Saudi Localization | 18 | 20 | Strong Saudi localization. "شريكك الموثوق في التحول الرقمي", Vision 2030 alignment, Saudi government certification, Saudi years in market. Minor: testimonial attribution is "إحدى شركات الاتصالات" not named — slight trust deduction |
| Persuasiveness | 12 | 15 | Good problem→solution→benefit→CTA structure. Numbers present (35% cost reduction, 200 clients, 15 years). Testimonial adds credibility. CTA is specific and low-friction |
| SEO Quality | 7 | 10 | Good keyword coverage ("التحول الرقمي", "شريكك الموثوق"). Clean structure. Could optimize meta description further. Missing schema markup opportunity |
| Authority & Trust | 8 | 10 | Good trust signals (15 years, 200 clients, 35% savings, government certification, testimonial). Deduction for anonymous testimonial company |
| Clarity | 9 | 10 | Clear value prop. Logical flow. Bulleted services. Easy to understand on first read |
| Readability | 4 | 5 | Good structure. Bullet points. Short sentences. Slight: testimonial could be formatted more distinctively |
| Conversion Potential | 4 | 5 | Excellent CTA ("احجز استشارة مجانية — ٣٠ دقيقة مع خبير تقني"). Low friction. Could add slight urgency for higher score |
| Originality | 3 | 5 | Well-executed but follows the standard Saudi tech formula. Not breaking new ground creatively. Some differentiation with the specific 35% number |
| **TOTAL** | **81** | **100** | **PASS — Good quality, minor improvements possible** |

**Strengths:** Strong Saudi localization, good trust signals, clear structure, effective CTA.
**Improvements:** Name the testimonial company, add urgency to CTA, improve meta description for SEO, add one unique angle for originality.

---

### Example 3: Premium Saudi Enterprise AI — "ذكاء الأعمال المتقدمة"

**Text:**
> تواجه البنوك السعودية تحدياً متزايداً: اكتشاف الاحتيال في وقت آني. ٦٢٪ من البنوك في المنطقة تستخدم أنظمة تقليدية تكتشف ٣٤٪ فقط من محاولات الاحتيال. نموذجنا يتفوق على هذه الأنظمة بنسبة اكتشاف ٩٧٪ مع ٢٪ فقط من النتائج الإيجابية الخاطئة.
>
> طورنا نموذجنا على بيانات معاملات حقيقية من ٣ بنوك سعودية على مدى ٨ سنوات. النموذج مدرب على ١٢ مليون معاملة ويُحدّث آنياً مع كل معاملة جديدة. يعمل مع البنية التحتية الحالية — لا حاجة لتغيير الأنظمة الموجودة.
>
> حصلنا على موافقة هيئة الاتصالات والفضاء والتقنية (CST) ونعمل مع صندوق الاستثمارات العامة في تطبيق النموذج في جهات حكومية. فريقنا يضم ٢٨ خبيراً في تعلم الآلة، ١٥ منهم يحملون دكتوراه من جامعات عالمية.
>
> قال الدكتور خالد القحطاني، الرئيس التنفيذي للتقنية في بنك الرياض: «نظام ذكاء الأعمال المتقدمة خفض الاحتيال بنسبة ٨٥٪ في أول ربع — بفارق كبير عن أي نظام آخر جربناه».
>
> احجز عرضاً توضيحياً مخصصاً — سنصمم نموذجاً تجريبياً على بياناتك في أسبوع واحد، بدون أي التزام مالي.

| Category | Score | Max | Rationale |
|----------|-------|-----|-----------|
| Naturalness | 20 | 20 | Fluent native Arabic. No translation artifacts. Natural sentence rhythm. Appropriate use of English terms (CST). Zero clichés. Reads as authoritative, expert content |
| Saudi Localization | 20 | 20 | Perfect Saudi localization. Saudi banks as clients, CST certification, PIF collaboration, Saudi doctor name and bank name, Vision 2030 context implicit (anti-fraud = supporting financial sector growth). Correct formality level |
| Persuasiveness | 15 | 15 | Exceptional persuasion. Problem (62% banks use outdated systems) → specific failure rate (34% detection) → solution (97% detection) → evidence (3 banks, 8 years, 12M transactions) → objection handling (works with existing infrastructure) → credentials (CST, PIF, 28 experts) → full-attribution testimonial → risk-reversal CTA (free trial on own data, no commitment). Every element present |
| SEO Quality | 8 | 10 | Strong keyword targeting ("اكتشاف الاحتيال في البنوك السعودية", "نظام كشف احتيال"). Good structure. Could add Arabic schema for Article and FAQ. Minor: more internal linking opportunities |
| Authority & Trust | 10 | 10 | Maximum trust signals. Specific numbers (62%, 34%, 97%, 2%, 12M, 28 experts, 15 PhDs). Named Saudi bank client (بنك الرياض). Saudi certifications (CST). PIF partnership. Full-attribution testimonial with photo-implied detail. Team credentials |
| Clarity | 10 | 10 | Crystal clear. First sentence states the problem. Immediate data. Logical flow. Each paragraph has one topic. Jargon explained naturally. Perfect clarity |
| Readability | 5 | 5 | Excellent readability. Short sentences (8–15 words). Varied paragraph lengths. Good rhythm. Numbers boldable. Testimonial formatted distinctively. Perfect RTL |
| Conversion Potential | 5 | 5 | Best practice CTA: specific, low-friction, risk-reversed ("بدون أي التزام مالي"), personalized ("على بياناتك"), time-boxed ("في أسبوع"). No pressure. Value clearly communicated |
| Originality | 5 | 5 | Highly original. Specific to this company's technology and experience. Unique angle (97% detection with 2% false positives). Not a single cliché. Could only be written by this specific company |
| **TOTAL** | **98** | **100** | **EXCELLENT — Premium quality content** |

**Why this scores 98:**
- 20/20 Naturalness: Native Arabic, no artifacts, perfect flow
- 20/20 Saudi Localization: Deeply Saudi — Saudi client, CST, PIF, Saudi bank name, correct Saudi formality
- 15/15 Persuasiveness: Every persuasion element executed perfectly
- 10/10 Authority: Maximum trust through specific, verifiable evidence
- Gap: Could add 2 points for SEO schema markup and internal linking for a perfect 100

---

## Quick Reference: Scoring Cheat Sheet

| Category | Max | Pass Threshold | Quick Check |
|----------|-----|---------------|-------------|
| Naturalness | 20 | ≥14 | Read aloud. Does it sound like a Saudi person wrote it? |
| Saudi Localization | 20 | ≥14 | Would this work only in Saudi Arabia, or anywhere? |
| Persuasiveness | 15 | ≥10 | Can you state the value proposition after one read? |
| SEO Quality | 10 | ≥7 | Is the primary keyword in H1 and meta? |
| Authority & Trust | 10 | ≥7 | Are claims backed by specific evidence? |
| Clarity | 10 | ≥7 | Can a non-technical reader understand it? |
| Readability | 5 | ≥4 | Would you want to read this on a phone? |
| Conversion Potential | 5 | ≥4 | Does the CTA make you want to click? |
| Originality | 5 | ≥3 | Could any competitor have written this? |

## Weighted Decision Matrix

For final Go/No-Go decisions on Arabic content:

1. **Check automatic rewrite triggers first.** Any trigger = No-Go.
2. **If no triggers, calculate weighted score.**
3. **Decision:**
   - 90–100: **Approve** — Publish as-is or with minor edits
   - 75–89: **Approve with edits** — Address identified gaps
   - 50–74: **Revise** — Targeted rewrite of underperforming categories
   - 0–49: **Reject** — Full rewrite from scratch
4. **Any single category at ≤50% of max:** Flag for review even if total passes.
   - Naturalness ≤10/20: Readers will detect non-native writing
   - Saudi Localization ≤10/20: Wrong market positioning
   - Persuasiveness ≤7/15: Content won't convert
