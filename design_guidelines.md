# DESIGN GUIDELINES: ConsumerShield UI/UX Standards

## 🎨 Brand Identity

### Brand Name
**ConsumerShield** - Professional, protective, empowering

### Brand Tagline
"Your money. Your rights. Our fight." (English)  
"Твои деньги. Твои права. Наша борьба." (Russian)

### Core Brand Values
- **Transparency:** No hidden fees, clear pricing upfront
- **Speed:** 10-30 day resolution (not 6-12 months)
- **Trust:** Licensed partnerships, guaranteed outcomes
- **Empowerment:** Consumers should feel control, not anxiety

---

## 🎨 Visual Identity

### Color Palette

| Color | Hex | Usage | Psychology |
|-------|-----|-------|-----------|
| **Primary Blue** | #1E40AF | CTAs, headers, buttons | Trust, law, professionalism |
| **Success Green** | #059669 | Success states, checkmarks, positive results | Growth, recovery, victory |
| **Warning Orange** | #EA580C | Alerts, important notices | Attention, action needed |
| **Neutral Gray** | #6B7280 | Text, backgrounds, borders | Balance, clarity |
| **Light Gray** | #F3F4F6 | Backgrounds, subtle divisions | Cleanliness, space |
| **Dark Charcoal** | #1F2937 | Body text, primary text | Readability, authority |

### Typography

#### Font Family: Inter (Google Fonts, free)
- **Usage:** All body text, UI, buttons
- **Reason:** Clean, modern, excellent readability on all devices

#### Font Sizes & Weights
```
Display (Hero):       Headline 1: 32px, Bold (700)
Large Heading:        Headline 2: 24px, Bold (700)
Section Heading:      Headline 3: 20px, Semibold (600)
Subheading:           Subtitle:   16px, Semibold (600)
Body Text:            Body:       14px, Regular (400)
Small Text:           Caption:    12px, Regular (400)
Button Text:          Button:     14px, Semibold (600)
```

### Logo Variations

**Logo A: Full Logo (Primary)**
```
[Shield Icon] ConsumerShield
(Shield = upside-down triangle representing protection)
```

**Logo B: Icon Only**
```
[Shield Icon] (for app icon, favicon)
```

**Logo C: Horizontal Lockup**
```
[Shield Icon] | ConsumerShield
(For header bar)
```

---

## 📐 Layout & Spacing

### Grid System
- **Base unit:** 4px
- **Column grid:** 12 columns on desktop, 4 on mobile
- **Gutters:** 16px (4 base units)

### Spacing Scale
```
xs:  4px   (tight spacing)
sm:  8px   (compact)
md:  16px  (normal)
lg:  24px  (comfortable)
xl:  32px  (generous)
2xl: 48px  (dramatic)
```

### Common Spacing Patterns
- Card padding: 24px (lg)
- Button padding: 12px (vertical) × 16px (horizontal)
- Section margins: 48px (2xl) top/bottom
- Mobile-first: Reduce by 50% on screens < 768px

---

## 🎯 UI Components

### Buttons

#### Primary Button (Main CTAs)
```
Background: #1E40AF (Primary Blue)
Text Color: White (#FFFFFF)
Padding: 12px × 16px
Border Radius: 8px
Font Weight: 600
State:
  - Default: Blue background
  - Hover: Darker blue (#1E3A8A)
  - Active: Even darker (#1F2937)
  - Disabled: Gray (#D1D5DB)
```

**Usage:** "Book Consultation", "Start Recovery", "Pay Deposit"

#### Secondary Button (Alternative)
```
Background: White (#FFFFFF)
Border: 2px solid #1E40AF
Text Color: #1E40AF
Padding: 12px × 16px
Border Radius: 8px
Font Weight: 600
```

**Usage:** "Learn More", "Cancel", "Edit"

#### Success Button (Confirmation)
```
Background: #059669 (Success Green)
Text Color: White
Padding: 12px × 16px
Border Radius: 8px
Font Weight: 600
```

**Usage:** "Confirm Payment", "Send Claim"

### Cards

```
Background: White
Border: 1px solid #E5E7EB
Border Radius: 12px
Padding: 24px
Box Shadow: 0 1px 3px rgba(0,0,0,0.1)
```

**Card Variants:**
- **Flat:** No shadow (simple)
- **Elevated:** Subtle shadow (emphasis)
- **Interactive:** Hover shadow effect

### Input Fields

```
Background: #F9FAFB
Border: 1px solid #D1D5DB
Border Radius: 8px
Padding: 12px
Font Size: 14px
Font Weight: 400
Placeholder Color: #9CA3AF

Focus State:
  Border: 2px solid #1E40AF
  Box Shadow: 0 0 0 4px rgba(30, 64, 175, 0.1)
```

### Alerts & Notifications

```
Success Alert:
  Background: #ECFDF5 (light green)
  Border: 1px solid #10B981
  Icon: ✓ (green)
  Text: #047857 (dark green)
  
Warning Alert:
  Background: #FFFBEB (light yellow)
  Border: 1px solid #FCD34D
  Icon: ⚠️ (orange)
  Text: #92400E (dark orange)
  
Error Alert:
  Background: #FEF2F2 (light red)
  Border: 1px solid #FCA5A5
  Icon: ✕ (red)
  Text: #991B1B (dark red)
```

---

## 📱 Responsive Breakpoints

```
Mobile:   < 640px   (phones)
Tablet:   640px - 1024px
Desktop:  > 1024px
```

### Mobile-First Adjustments
- **Font sizes:** Reduce by 10-15% on mobile
- **Spacing:** Reduce padding/margins by 50%
- **Cards:** Stack vertically (100% width)
- **Buttons:** Full width on mobile
- **Navigation:** Hamburger menu (mobile), horizontal (desktop)

---

## 🎬 User Interface Screens

### Screen 1: Telegram Channel
```
[Header]
ConsumerShield - Защита прав потребителей
Подписчики: 500+ | Следить

[Daily Tips Feed]
📌 ПН: "Товар не работает? Это БРАК! Вот как его вернуть"
  └─ [9 сек видео] + [Ссылка на консультацию]

📌 ВТ: "5 правил возврата товара за деньги"
  └─ [List with checkmarks]

📌 СР: "Компания игнорирует претензию? Вот что делать"
  └─ [Action steps + button]

[Bottom Navigation]
[Book Consultation] [FAQ] [Chat Support]
```

### Screen 2: Consultation Booking
```
[Header]
Консультация: 1,500 РУБ (30 минут)

[Form]
Ваше имя: [________]
Телефон: [________]
Краткое описание проблемы: [_______________]
Загрузить фото документов: [Upload Photos]

[Success Probability Estimate (AI Generated)]
📊 Вероятность успеха: 78% ✅
   Основано на анализе 1,000+ похожих дел

[Booking Calendar]
Доступные время:
○ Сегодня 14:00
○ Завтра 10:00
○ Завтра 15:00

[CTA Button]
[Подтвердить консультацию] (Primary button)
```

### Screen 3: Payment Confirmation
```
[Header]
Подтверждение платежа

[Order Summary]
┌─────────────────────────┐
│ Консультация            │
│ 1,500 РУБ              │
│                        │
│ Способ оплаты: Карта    │
│ Статус: Обработка...    │
└─────────────────────────┘

[Zoom Link - After Payment]
✅ Платеж принят!

Ваша консультация начинается в:
[Timer showing 5 minutes]

[Copy Zoom Link] [Join Now]
```

### Screen 4: Claim Generation Result
```
[Header]
Анализ вашего дела

[AI Analysis Card]
🤖 АНАЛИЗ ДОКУМЕНТОВ (Claude AI)

Загруженные:
✓ Чек покупки
✓ Гарантийный лист
✓ Письмо компании с отказом

Вероятность успеха: 82%
Основной закон: "О защите прав потребителей" (статья 18)

Рекомендация: ✅ БЕРЕМ ДЕЛО
```

[Claim Letter Generated]
```
ПРЕТЕНЗИЯ О ВОЗВРАТЕ ТОВАРА

Уважаемые представители ООО "Компания"

Я, [Ваше имя], приобрел(а) товар:
- Товар: [Название]
- Дата покупки: [Дата]
- Стоимость: [Сумма]
- Выявленный дефект: [Описание]

Требую возврата денежных средств в размере [Сумма] РУБ
в соответствии с Законом РФ "О защите прав потребителей".

[Download PDF] [Send to Company] [Proceed to Deposit]
```

### Screen 5: Deposit Payment
```
[Header]
Депозит для начала работы

[Payment Calculation]
📊 РАСЧЕТ КОМИССИИ

Сумма возврата (ожидаемо): 50,000 РУБ
Ваш депозит (30%): 15,000 РУБ
Наша комиссия (25%): 12,500 РУБ
Ваша чистая выплата: 37,500 РУБ

✅ Гарантия: Если проиграем,
   вернём 50% депозита (7,500 РУБ)
```

[Payment Options]
```
● Yandex.Kassa (карта/счет)
● Сбербанк (прямой перевод)
● Контакт (если в Казахстане)
```

[Payment Summary]
```
[Pay 15,000 RUB] (Primary button)
[Cancel] (Secondary button)
```

---

## 🎨 Color Application Examples

### Success State (Case Approved)
```
✅ Дело успешно начато!

[Green card with success icon]
Наш консультант начал работу над вашим делом.
Вы получите обновление через 24 часа в этом чате.

Ожидаемый результат: 50,000 РУБ
Ожидаемое время: 10-30 дней
```

### Warning State (Case on Hold)
```
⚠️ Требуется действие

[Orange card with warning icon]
Нам нужны дополнительные документы:
- Копия гарантийного талона
- Переписка с компанией

[Upload Documents] (Primary button)
```

### Error State (Issue)
```
❌ Ошибка обработки платежа

[Red card with error icon]
Платеж не прошел. Пожалуйста, попробуйте снова.
Код ошибки: PAYMENT_DECLINED

[Try Again] (Primary button)
[Contact Support] (Secondary button)
```

---

## 📲 Mobile-Specific Design

### Hamburger Navigation (Mobile)
```
[☰] ConsumerShield      [?]
────────────────────────────
│ Dashboard
│ My Cases
│ Wallet
│ Settings
│ Help & Support
│ Log Out
────────────────────────────
```

### Bottom Navigation Tab (Alt Design)
```
┌──────────────┬──────────────┬──────────────┐
│   🏠 Home    │   📁 Cases   │   👤 Profile │
└──────────────┴──────────────┴──────────────┘
```

### Mobile Form (Full Width)
```
┌──────────────────────────┐
│ КОНСУЛЬТАЦИЯ: 1,500 РУБ  │
├──────────────────────────┤
│                          │
│ Ваше имя:               │
│ [____________________]  │
│                          │
│ Телефон:                │
│ [____________________]  │
│                          │
│ Описание проблемы:       │
│ [_________________      │
│  ________________       │
│  ________________]      │
│                          │
│ [ПОДТВЕРДИТЬ]           │
│                          │
└──────────────────────────┘
```

---

## ♿ Accessibility Standards

### WCAG 2.1 AA Compliance
- **Color Contrast:** Minimum 4.5:1 for all text
- **Font Size:** Minimum 14px for body text
- **Alt Text:** All images have descriptive alt text
- **Keyboard Navigation:** All functions accessible via keyboard
- **Focus Indicators:** Clear focus states on interactive elements

### Accessibility Checklist
- ✅ Buttons have sufficient size (minimum 44×44 px on mobile)
- ✅ Forms have clear labels + error messages
- ✅ Videos have captions (Telegram videos, TikToks)
- ✅ Color not the only indicator of status (use icons too)
- ✅ Loading states are clear (not just spinner)

---

## 🎥 Animation & Transitions

### Micro-interactions

**Button Hover Effect:**
```
Duration: 150ms
Effect: Scale 1.02x + Slight shadow increase
```

**Payment Success:**
```
Checkmark animation: 300ms
Confetti effect: 1 second
Success message fade-in: 200ms
```

**Form Validation:**
```
Error shake: 200ms
Error message slide-in: 150ms
Success checkmark fade: 100ms
```

### General Guidelines
- Keep animations under 300ms for responsiveness
- Use ease-out for entrance, ease-in for exit
- Avoid animations that distract from content
- Mobile: Reduce or disable animations for performance

---

## 📋 Typography Hierarchy

### Example Page Layout

```
HERO SECTION (Display 1 - 32px Bold)
Верни свои деньги за брак товара

Подзаголовок (Subtitle - 16px Semibold)
За 10-30 дней без судов

[Primary Button]


SECTION HEADING (Headline 2 - 24px Bold)
Как это работает?

Body text (14px Regular)
Процесс состоит из 3 этапов: консультация,
претензия, и если нужно - суд.

Subsection (Headline 3 - 20px Semibold)
Этап 1: Консультация

Detailed explanation (14px Regular)
На консультации мы анализируем ваши документы
и определяем вероятность успеха...
```

---

## 🌐 Localization Notes (For Future)

Currently: Russian-only (Russia focus)

**Future expansions:**
- Ukrainian (similar legal framework, diaspora)
- Kazakh (CIS market, Russian-speaking)
- English (international diaspora)

**Localization guidelines:**
- Right-to-left not needed (Cyrillic scripts are LTR)
- Character encoding: UTF-8 throughout
- Date format: DD.MM.YYYY (Russian standard)
- Number format: 1 234,56 (space as thousands separator)
- Currency: РУБ always displayed

---

## 📐 Design Specifications Summary

| Element | Size | Color | Font | Weight |
|---------|------|-------|------|--------|
| Button (Primary) | 44×12px pad | #1E40AF | Inter | 600 |
| Input Field | 40px height | #F9FAFB | Inter | 400 |
| Card | 24px pad | White | - | - |
| Heading 1 | 32px | #1F2937 | Inter | 700 |
| Body Text | 14px | #6B7280 | Inter | 400 |

---

**Design Guidelines Version:** 1.0  
**Status:** ✅ READY FOR DEVELOPMENT  
**Designer Notes:** All components built for accessibility + mobile-first responsiveness
