# METHOD — North Star Metric (Sean Ellis)

> מדד יחיד שמייצג את כל בריאות העסק. **Sean Ellis** (אבי ה-Growth Hacking, מי שטבע את המונח) זיהה ש-הסטארטאפים שצמחו הכי מהר היו אלה ש**הצליחו לבחור מדד אחד שכולם — מהמייסד עד המתכנת — מבינים ושואפים אליו**.

## העיקרון

### למה מדד יחיד?
**בעיה:** עסק עם 15 מדדים = אף אחד לא יודע מה חשוב באמת.

**פתרון:** North Star Metric (NSM) — *"הדבר היחיד שאם נכפיל אותו → העסק שלנו מצליח."*

### מה מאפיין NSM טוב?

| ✅ | ❌ |
|---|---|
| משקף Value Delivered ללקוח | מודד פעילות פנימית בלבד (e.g. "מספר עובדים") |
| Leading Indicator (חזה את הכנסה עתידית) | Lagging (הכנסה ה-המ historic) |
| מעלה כמעט בודאות עם הצלחה | יכול לעלות גם בכישלון (e.g. "Signups" עולה אבל Churn גבוה) |
| כל הצוות מבין | מורכב, דורש הסבר |
| ניתן להשפיע ישירות | תלוי בגורמים חיצוניים |
| Cumulative או Time-bound | חד-פעמי |

## דוגמאות מהשטח

| חברה | North Star Metric | למה זה עובד |
|------|--------------------|--------------|
| **Airbnb** | Nights Booked | משקף ערך ללקוח + הכנסה |
| **Facebook** | Daily Active Users (DAU) | Engagement = Network effect = ad revenue |
| **Spotify** | Time Spent Listening | Engagement = retention = subscription |
| **WhatsApp** | Messages Sent | Network value = retention |
| **Slack** | Number of Messages Sent within Team | Team adoption = retention + expansion |
| **Quora** | Useful Answers per Quarter | Quality content = traffic + monetization |
| **Amazon** | Items Purchased per Month | Frequency = revenue |
| **Tesla** | Vehicles Delivered | Production capacity = revenue |
| **Netflix** | Hours Streamed per User per Month | Engagement = retention |

## איך בוחרים NSM (תהליך 5 שלבים)

### שלב 1: רשום 5-10 candidates
- הכנסה? לא — Lagging.
- Signups? לא — לא משקף Value.
- *"Active users שמשתמשים פיצ'ר X לפחות 3 פעמים בשבוע"* — אולי.

### שלב 2: לכל candidate, ענה:
- **האם הוא משקף Value ללקוח?** (קריטריון #1)
- **האם הוא Leading Indicator?**
- **האם הוא בלתי-ניתן-לזיוף?** (אם אני סופר signups, יכול להעלות בלי ערך)
- **האם הוא Time-bound?** (אם cumulative בלבד, יחזיק לנצח)

### שלב 3: דווח לצוות + שאל
- **שאלה:** *"אם זה היה המדד היחיד שאתה רואה בכל בוקר — היית מצליח לעבוד טוב?"*
- אם רוב הצוות אומר "כן" → סימן טוב.

### שלב 4: בדוק קורלציה היסטורית
- האם בחודשים שה-NSM עלה — הכנסה עלתה?
- אם לא — לא NSM טוב.

### שלב 5: הצהר עליו + מדוד שבועי
- כל פגישה צוות מתחילה ב-NSM.
- כל החלטה גדולה — *"איך זה משפיע על ה-NSM?"*

## NSM לעסקי שירות

עסק שירות שונה מ-SaaS. ה-NSM צריך לשקף תוצאת לקוח.

### לפי סוג עסק

| סוג | NSM מתאים |
|------|------------|
| **Coaching / Consulting** | Active paying clients × NPS |
| **Agency / Done-for-you** | Recurring monthly revenue × Avg client tenure |
| **Course / Education** | Active learners completing milestones |
| **Community / Membership** | Active members × Engagement Rate |
| **B2B Services** | Annual Contract Value × Renewal Rate |

## הסכנה הקלאסית — Vanity Metrics

**Vanity Metric** = מספר שעולה, נראה טוב, **אבל לא משקף ערך**.

דוגמאות:
- **Page Views** — יכול לעלות מ-bots / SEO רעב, בלי Conversion.
- **Signups** — אם 80% נוטשים תוך 7 ימים, זה לא ערך.
- **Followers על Social** — בלי engagement, בלי conversion.
- **Total Customers** — אם churn גבוה, אין באמת growth.

**מבחן:** אם המדד יכול לעלות בלי שהעסק מצליח → vanity.

## NSM ↔ Sub-Metrics

ה-NSM הוא הר. כדי להעלות אותו, צריך לעבוד על **sub-metrics** שמרכיבים אותו.

**דוגמה — Airbnb:**
```
North Star: Nights Booked

Sub-metrics:
├── New users acquired (Top-of-funnel)
│   ├── Marketing spend → Conversion to signup
├── Activation (New users → First booking)
│   ├── Onboarding completion
│   ├── First booking within 30 days
├── Retention (Repeat bookings)
│   ├── 2nd booking within 90 days
│   ├── Cohort retention rate
└── Revenue per booking
    ├── Avg nightly rate
    ├── Service fees
```

לעלות את ה-NSM = לעבוד על sub-metric אחד מהאלה.

## הקשר ל-Methods אחרים

- [Pirate Funnel](pirate-funnel.md) — כל "A/R" שם הוא sub-metric ל-NSM.
- [Cohort Tracking](../tools/cohort-tracking.md) — איך מודדים את ה-NSM לאורך זמן.
- [EOS Scorecard](eos-scorecard.md) — Scorecard יכול לכלול את ה-NSM + 5-10 sub-metrics.

## הספרים והמקורות
- *Hacking Growth* — Sean Ellis + Morgan Brown (2017) ⭐
- *Lean Analytics* — Croll & Yoskovitz (מסביר Vanity vs Actionable Metrics)
- *Measure What Matters* — John Doerr (OKRs, משלים)

## דוגמה — NSM למאמן עסקי

**מועמדים:**
1. *"מספר לקוחות פעילים"* — לא משקף איכות.
2. *"הכנסה חודשית"* — Lagging.
3. *"מספר לקוחות שהשיגו את ה-Big Rock שלהם בקוהורט"* — ⭐
4. *"NPS"* — חצי-NSM (טוב, אבל לא מספיק כצפי).

**הבחירה:** *"מספר לקוחות שהשיגו את ה-Big Rock שלהם בכל קוהורט × NPS שלהם."*

**למה זה עובד:**
- משקף Value (Big Rock = תוצאה).
- Leading (אם הם משיגים → recurring + referrals).
- בלתי-ניתן-לזיוף (Big Rock מוגדר מראש, NPS חיצוני).
- Time-bound (כל קוהורט = 3-6 חודשים).
- כל הצוות מבין.

## היסטוריית גרסאות
- 2026-06-01: כתיבה ראשונה.
