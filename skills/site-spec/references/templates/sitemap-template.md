# מפת אתר + Exit-Paths — [שם לקוח]

> **חוק הזהב:** כל עמוד, כל section, כל widget — חייב exit-path. אין cul-de-sacs.

---

## 1. רשימת עמודים

```
/                       בית / Home
/product                מוצר / שירות
/[sub-service-a]        שירות משני A
/[sub-service-b]        שירות משני B
/about                  על
/contact                צור קשר
/thank-you              תודה (אחרי שליחת טופס)
/landing/[campaign-1]   דף נחיתה לקמפיין 1
/landing/[campaign-2]   דף נחיתה לקמפיין 2
/blog                   בלוג (אופציונלי)
/blog/[post]            פוסט בבלוג
```

---

## 2. היררכיה

```
Home (/)
├── Product (/product)
│   ├── Sub-service A (/sub-service-a)
│   └── Sub-service B (/sub-service-b)
├── About (/about)
├── Contact (/contact)
├── Blog (/blog)
│   └── Post (/blog/[slug])
└── Landing pages (external to main nav)
    ├── /landing/campaign-1
    └── /landing/campaign-2
```

**כלל:** כל עמוד <=3 קליקים מהבית.

---

## 3. טבלת Exit-Paths ⭐

| עמוד | CTA ראשי | CTA משני | פוטר (תמיד) | קישורים פנימיים |
|------|-----------|-----------|--------------|-------------------|
| `/` | [פעולה + לאן] | [פעולה + לאן] | טופס מקוצר + WhatsApp | product, testimonials, about |
| `/product` | | | ⬆️ | home, contact, sub-services |
| `/sub-service-a` | | | ⬆️ | product, contact |
| `/about` | | | ⬆️ | product, contact |
| `/contact` | שליחת טופס → /thank-you | WhatsApp | ⬆️ | (עמוד לכידה — מינימום הסחות) |
| `/thank-you` | לינק לעמוד תוכן נוסף | הזמנה לוואטסאפ | ⬆️ | product, about, blog |
| `/blog/[post]` | CTA ראשי ל-product/contact | הרשמה לניוזלטר | ⬆️ | 2-3 פוסטים קשורים |
| `/landing/...` | [CTA ייעודי לקמפיין] | WhatsApp | ⬆️ (מצומצם) | ❌ אין תפריט ראשי |

**Red flags (לא לקבל איפיון עד שתוקנו):**
- ❌ עמוד בלי CTA ראשי
- ❌ CTA משני = "חזור לבית"
- ❌ `/thank-you` שמסיים ב-"תודה" בלי CTA להמשך
- ❌ דפי נחיתה עם תפריט ראשי (מוריד המרה)

---

## 4. Flow של גולש — 3 תרחישים

### Flow 1 — אווטאר ראשי מ-Meta (קהל קר)

```
Meta ad →
  /landing/[avatar-1-campaign] →
    [קורא הוק + רואה offer] →
      CTA: "בוא נדבר" →
        /thank-you →
          [WhatsApp prefilled או המתנה לשיחת חזרה]
```

**נקודות leak אפשריות + פתרון:**
- ב-Hero: לא מזוהה → סרגל trust למעלה + H1 ספציפי לאווטאר
- אחרי הוק: לא ממשיך → mini-CTA באמצע העמוד
- בטופס: נוטש → WA fallback + מינימום שדות

### Flow 2 — אווטאר ראשי מגוגל (search intent)

```
Google Search →
  /product (או /sub-service-a) →
    [רואה תשובה לחיפוש] →
      CTA: "קבל הצעה" →
        /contact →
          /thank-you
```

### Flow 3 — קהל חם (referral / ישיר)

```
Direct / Referral →
  / (home) →
    [רואה Value Stack + עדויות] →
      CTA: "תתחיל" →
        /contact או WhatsApp →
          /thank-you
```

---

## 5. דפי נחיתה קמפיינים

### `/landing/[campaign-slug]` — תבנית

**יעד:** המרה יחידה. בלי הסחות.

**מבנה מינימליסטי:**
1. Hero ממוקד קמפיין (H1 שתואם מודעה)
2. הוכחה מהירה (3 לוגואים / מספר לקוחות)
3. Value Prop 3-4 bullets
4. CTA ראשי
5. 2-3 עדויות
6. FAQ קצר (3-4 שאלות)
7. Final CTA + Risk Reversal
8. פוטר מינימלי

**מה **אין**:**
- ❌ תפריט ראשי
- ❌ קישורים חוצים לאתר הראשי
- ❌ לינק לבלוג / about

**UTMs:** כל קישור למודעה חייב UTM מלא (source / medium / campaign / content / term + fbclid/gclid).

---

## 6. עמודי "עזר" (לא מכירה)

| עמוד | תפקיד | Exit-Path |
|------|--------|-----------|
| `/privacy` | משפטי — GDPR/פרטיות | חזרה לעמוד הקודם |
| `/terms` | משפטי — תנאי שימוש | חזרה לעמוד הקודם |
| `/404` | שגיאה | לינקים ל-3 עמודי תוכן מרכזיים + CTA ראשי |

**`/404` חובה לא להיות dead-end** — מי שהגיע לשם הוא ליד פוטנציאלי.

---

## 7. Checklist הגשה

- [ ] כל עמוד בטבלה מולא במלואו (CTA ראשי + משני + פוטר + קישורים)?
- [ ] אין עמוד בלי CTA ראשי?
- [ ] `/thank-you` מחזיר את הגולש לפאנל ולא "תודה עד כאן"?
- [ ] `/404` הוא לא dead-end?
- [ ] דפי הנחיתה בלי תפריט ראשי?
- [ ] UTMs + hidden fields הוגדרו לכל טופס?
- [ ] 2-3 flows של גולשים מעודכנים ותואמים את המפה?
