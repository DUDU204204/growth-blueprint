# METHOD — Unit Economics (Lean Startup)

> השאלה הכי חשובה ב-business: **"כמה אני מרוויח מלקוח אחד, בניכוי כמה עלה להשיג אותו?"** אם המספר שלילי — כל אסטרטגיית הצמיחה חסרת משמעות.

## העיקרון

**Eric Ries** ב-*The Lean Startup* (2011): סטארטאפ יכול לצמוח שנים בלי לדעת שהוא **מפסיד על כל לקוח**. לקוחות חדשים מסתירים את האמת.

ה-Unit Economics חושף את האמת **לפני שזה מאוחר**.

## המשוואה הבסיסית

```
Contribution Margin per Unit = LTV - CAC
```

**אם > 0 = ה-business פעיל.**  
**אם < 0 = כל לקוח עולה לך כסף. אתה גוסס.**

### המספרים בפירוט

```
                    Revenue per Customer    ←  ARPU × Months Retained
                  -  COGS per Customer       ←  עלות מסירת המוצר/שירות
                  -  Variable costs           ←  Stripe fees, hosting, etc.
                  ─────────────────────────
LTV (Net)         =  Gross Profit per Customer

CAC               =  Total Marketing+Sales Spend
                     ────────────────────────────
                     New Customers Acquired

Unit Economics    =  LTV - CAC
```

## הבנצ'מרק לעסק בריא

| יחס | מה זה אומר |
|------|------------|
| **LTV / CAC ≥ 3** | בריא. כל ₪1 בשיווק → ₪3 חזרה. |
| **LTV / CAC ≥ 5** | חזק. תוכל להגדיל השקעה בשיווק. |
| **LTV / CAC < 3** | אזעקה. לא בר-קיימא ארוך-טווח. |
| **LTV / CAC < 1** | מפסיד על כל לקוח. הצמיחה תהרוג אותך. |

| Payback period | מה זה אומר |
|-----------------|------------|
| **< 6 חודשים** | מעולה. הון מתחזק במהירות. |
| **6-12 חודשים** | בריא. רוב העסקים. |
| **12-24 חודשים** | דורש מימון. SaaS Enterprise. |
| **> 24 חודשים** | סיכון מימוני גבוה. |

## איך מחשבים בעסק שירות

### LTV — Lifetime Value

```
LTV = ARPU × Avg Customer Lifetime
```

**דוגמה:** ליווי עסקי ₪5,000/חודש, ממוצע 6 חודשים → LTV = ₪30,000.

**שיפור LTV:**
- ARPU גבוה יותר (Premium tier).
- Lifetime ארוך יותר (Onboarding טוב, retention).
- Continuity אחרי הליווי.

### CAC — Customer Acquisition Cost

```
CAC = (Marketing + Sales spend בתקופה) / לקוחות חדשים באותה תקופה
```

**מה לכלול ב-CAC:**
- ✅ Paid ads (Meta, Google).
- ✅ Tools שכרוך בו (CRM, mailings).
- ✅ זמן sales team (× שכר).
- ✅ Commissions / Referral fees.
- ✅ זמן היזם (אם sales-led).

**מה לא לכלול:**
- ❌ Salary של עובדים שלא בשיווק/מכירות.
- ❌ Office, rent.
- ❌ Product development.

### דוגמה — מאמן עסקי

```
חודש ינואר:
- Meta ads: ₪8,000
- LinkedIn ads: ₪2,000
- VA SDR (50% מזמן): ₪3,000
- CRM (TickTick / Calendly): ₪200
- זמן היזם בשיחות אבחון (10h × ₪500 hour): ₪5,000
- סה"כ Marketing+Sales: ₪18,200

לקוחות חדשים: 4

CAC = ₪18,200 / 4 = ₪4,550

LTV (חישוב מ-cohort historic):
- ARPU: ₪5,000/חודש
- Avg lifetime: 6 חודשים
- LTV: ₪30,000

LTV / CAC = 30,000 / 4,550 = 6.6 ✅ חזק
Payback period: ₪4,550 / ₪5,000 = 0.9 חודש ✅ מעולה
```

## הטעות הקלאסית — Topline Growth Trap

חברה גדלה ב-Revenue 100% בשנה — נראה מעולה. בפועל:
- LTV: ₪10,000
- CAC: ₪15,000
- כל לקוח חדש = הפסד של ₪5,000.
- שנה 1: 10 לקוחות → -₪50,000 הפסד.
- שנה 2: 100 לקוחות (10x) → -₪500,000 הפסד.

**הצמיחה הכפילה את ההפסד.**

## איך מתקנים Unit Economics רעות

### אסטרטגיה 1 — הגדל LTV
**4 דרכים** (ראה גם [LTV Multiplier](../tools/ltv-multiplier.md)):
- Frequency — מוצרים חוזרים.
- ARPU — Premium tiers.
- Lifetime — Onboarding + Retention.
- Referrals — Word-of-mouth = CAC=0.

### אסטרטגיה 2 — הקטן CAC
- Organic channels (SEO, Content).
- Referral program — viral coefficient.
- Self-serve onboarding (ב-SaaS).
- Better targeting → less waste in ads.

### אסטרטגיה 3 — Disqualify לקוחות גרועים
- 20% מהלקוחות = 80% מההוצאות התפעוליות.
- ראה [Disqualification Criteria](../tools/disqualification-criteria.md).

## Cohort Unit Economics

האמת היחידה — חלוקת Unit Economics לפי **קוהורט**.

```
Cohort | LTV  | CAC   | LTV/CAC | Payback | סטטוס |
-------|------|-------|---------|---------|--------|
Q1 2026| 25K  | 5K    | 5x      | 1.0 mo  | ✅     |
Q2 2026| 28K  | 5.5K  | 5.1x    | 1.1 mo  | ✅     |
Q3 2026| 30K  | 7K    | 4.3x    | 1.4 mo  | 🟡     |
Q4 2026| 22K  | 12K   | 1.8x    | 2.5 mo  | ❌     |
```

**מה רואים:** Q4 התדרדר. בדיקה:
- CAC עלה (יותר תחרות?)
- LTV ירד (cohort בעייתי?)
- שינוי בערוצים?

זה ה-data ש**מקדים אזעקה**, לפני שזה מופיע ב-P&L.

## הקשר ל-Methods אחרים

- [LTV Multiplier](../tools/ltv-multiplier.md) — איך מעלים את ה-LTV.
- [Cohort Tracking](../tools/cohort-tracking.md) — איך מודדים Unit Economics לאורך זמן.
- [Paid Launch Checklist](../tools/paid-launch-checklist.md) — לוודא ש-CAC לא בורח.
- [Disqualification Criteria](../tools/disqualification-criteria.md) — הקטנת operational CAC.

## הספרים והמקורות
- *The Lean Startup* — Eric Ries (2011) ⭐ — מקור המונח
- *Hacking Growth* — Sean Ellis (חישוב CAC מפורט)
- *Predictable Revenue* — Aaron Ross (Outbound CAC)
- *Demand-Side Sales 101* — Bob Moesta

## מבחן מהיר — Unit Economics של העסק שלי

```
שלב 1: ARPU חודשי = ___
שלב 2: ממוצע חודשים שלקוח נשאר = ___
שלב 3: LTV = ARPU × חודשים = ___
שלב 4: CAC (3 חודשים אחרונים, ממוצע) = ___
שלב 5: LTV / CAC = ___

אם > 3: ✅ בר-קיימא. הגדל השקעה.
אם 1-3: 🟡 רגיש. שפר LTV או CAC.
אם < 1: ❌ אזעקה. עצור לפני שהצמיחה תקטל אותך.
```

## היסטוריית גרסאות
- 2026-06-01: כתיבה ראשונה.
