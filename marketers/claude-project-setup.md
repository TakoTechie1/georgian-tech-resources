# Claude Project — სრული Setup გაიდი ქართული მცირე ბიზნესისთვის

> 30-წუთიანი setup, რომელიც Claude-ს გადააქცევს თქვენი ბრენდის voice-ის მცოდნე ასისტენტად. ჩაგდე ერთხელ — Claude უკვე ცნობს თქვენს ბიზნესს ყოველ ჩათში.

**ავტორი:** [TakoTechie1](https://github.com/TakoTechie1)
**ლიცენზია:** MIT — თავისუფლად გამოიყენე და გააზიარე
**ბოლო განახლება:** 2026

---

## 📚 სარჩევი

- [რა გჭირდება](#რა-გჭირდება)
- [ნაბიჯი 1 — Project-ის შექმნა](#ნაბიჯი-1--project-ის-შექმნა)
- [ნაბიჯი 2 — Custom Instructions (System Prompt)](#ნაბიჯი-2--custom-instructions-system-prompt)
- [ნაბიჯი 3 — Brand Voice Worksheet](#ნაბიჯი-3--brand-voice-worksheet)
- [ნაბიჯი 4 — Reference Docs](#ნაბიჯი-4--reference-docs)
- [10 Starter Prompt](#10-starter-prompt)

---

## რა გჭირდება

- **Claude Pro** გამოწერა (ან Max / Team / Enterprise) — Projects-ის ფუნქცია მხოლოდ ფასიან გამოწერაშია
- **30 წუთი** ერთჯერადი setup-ისთვის
- **შენი ბრენდის ძირითადი ინფორმაცია** — სახელი, ნიშა, აუდიტორია, ტონი

---

## ნაბიჯი 1 — Project-ის შექმნა

1. გახსენი [claude.ai](https://claude.ai)
2. მარცხენა მენიუში დააჭირე **„Projects"**
3. დააჭირე **„New Project"**
4. დაარქვი — მაგალითად: „ჩემი ბრენდი 2026" ან კონკრეტული კლიენტის სახელი

> 💡 თუ რამდენიმე კლიენტი გყავს — თითოეულისთვის შექმენი ცალკე Project.

---

## ნაბიჯი 2 — Custom Instructions (System Prompt)

Project-ის შექმნისთანავე გაიხსნება „Custom Instructions" ველი. ჩასვი ქვემოთ მოცემული შაბლონი და შეცვალე ფიგურულ ფრჩხილებში მოცემული ცვლადები შენი ბრენდის მონაცემებით.

```
შენ ხარ [BRAND] ბრენდის Senior Marketing Specialist.

ბრენდის შესახებ:
→ სახელი: [BRAND NAME]
→ ნიშა: [მაგ. specialty coffee, fitness, beauty]
→ მდებარეობა: [Tbilisi, რაიონი]
→ სამიზნე აუდიტორია: [ვინ ყიდულობს — ასაკი, ინტერესი, საჭიროება]
→ მთავარი value proposition: [რა გადაწყვეტილებას აძლევთ კლიენტს]

ბრენდის voice:
→ ტონი: [მაგ. თბილი, professional, casual, fun]
→ ენის სტილი: [ქართული primary, English რჩევით]
→ რა სიტყვებს არ ვიყენებთ: [მაგ. cliché, jargon, „revolutionary"]

შენი როლი:
1. ყოველი წერილობითი output ჩვენი ბრენდის voice-ით
2. SEO meta, social posts, ad copy — ქართულად, არა Google Translate-ით
3. Call-to-action ბუნებრივად ჩართე ფინალში
4. Reference docs-ს გადახედე ყოველ ჯერზე — იქ არის ჩვენი ფაქტობრივი მონაცემები

თუ რამე გაუგებარი ან არასაკმარისად დაკონკრეტებულია, ჩემს მიერ მოწოდებული მონაცემები ვერ გყოფნის — გვეკითხე, არ მოიფიქრო.
```

> 💡 დაიმახსოვრე: რაც უფრო კონკრეტულია ცვლადები, მით უკეთესი იქნება output-ი. „თბილისური ბიზნესი" — ცუდი მაგალითია, „ვაკეში მდებარე specialty coffee roastery, რომელიც single-origin მარცვალს იყენებს" — სასურველი დონე.

---

## ნაბიჯი 3 — Brand Voice Worksheet

სანამ Custom Instructions-ში ჩვლადებს შეავსებ, უპასუხე ამ 5 კითხვას. პასუხები გადააქციე system prompt-ის მონაცემებად.

### 1. შენი ბრენდი best-friend-ია — რა ფრაზაში გადმოსცემ ამას?

```
[შენი პასუხი]
```

### 2. რა სიტყვა ნამდვილად შენი ბრენდი არ არის?

(მაგ. „luxury", „revolutionary", „synergy", „cutting-edge")

```
[შენი პასუხი]
```

### 3. ერთ წინადადებაში — რას აძლევ კლიენტს, რასაც კონკურენტი ვერ აძლევს?

```
[შენი პასუხი]
```

### 4. რა ემოცია უნდა იცვალოს კლიენტმა შენი content-ის წაკითხვის შემდეგ?

(მაგ. ნდობა, ცნობისმოყვარეობა, კომფორტი, ინსპირაცია, შვება)

```
[შენი პასუხი]
```

### 5. შენი 3 best customer-ის სახელი + 1 წინადადება მათზე

```
1. [სახელი] — [ერთი წინადადებით ვინ არის]
2. [სახელი] — [ერთი წინადადებით ვინ არის]
3. [სახელი] — [ერთი წინადადებით ვინ არის]
```

---

## ნაბიჯი 4 — Reference Docs

Project-ში მარცხენა მხარეს გაქვს „Project knowledge" სექცია — იქ ატვირთე ფაილები. Claude ცნობს თქვენს ბრენდს მხოლოდ იმდენად, რამდენადაც მონაცემს მისცემთ.

**აუცილებელი ფაილები:**

- ✅ **Brand guideline** — ლოგო, ფერები, typography, ტონის გაიდი (PDF ან image)
- ✅ **Customer personas** — 3-5 typical client აღწერა (ვინ არიან, რას ეძებენ, რა აშინებთ)
- ✅ **Product / service catalog** — ფასები, აღწერები, განსხვავებები
- ✅ **Past best campaigns** — რომელმა ad copy ან post იმუშავა — რატომ
- ✅ **FAQ answers** — ყველაზე ხშირი 10-15 კითხვა + სრული პასუხები
- ✅ **Top 10 customer reviews** — 5 დადებითი + 5 უარყოფითი (ცოცხალი ენით)
- ✅ **Style examples** — ლინკები ბრენდებზე, რომელთა voice მოგწონს

> 💡 თუ ყველა ფაილი ერთბაშად ვერ გაქვს მზად — დაიწყე 2-3 ფაილით (brand guideline + customer personas + FAQ). დანარჩენი დაამატე როგორც გაქვს დრო.

---

## 10 Starter Prompt

შემდეგი 10 prompt-ი გათვლილია იმისთვის, რომ Project-ის შექმნისთანავე დაუყოვნებლივ გამოიყენო. ცვლადები ფიგურულ ფრჩხილებშია.

### Prompt 1 — Meta Description Batch

```
დაწერე 5 meta description ქართულად ჩვენი [PRODUCT]-ისთვის.
150-160 სიმბოლო თითოეული, target keyword 1-ჯერ, CTA ფინალში.
```

### Prompt 2 — FB Ad Copy 5 Angles

```
დაწერე 5 Facebook ad copy ვარიაცია [PRODUCT]-ისთვის.
თითო — სხვა angle-ზე: FOMO, social proof, curiosity, transformation, ავტორიტეტი.
თითო max 90 სიმბოლო. CTA ბოლოს.
```

### Prompt 3 — Instagram Caption

```
დაწერე Instagram-ის caption [PRODUCT/POST]-ისთვის.
Hook პირველ ხაზში, value middle-ში, CTA ბოლოს.
ბრენდის ტონი — ჩემი reference-ის მიხედვით.
```

### Prompt 4 — Positive Review Reply

```
უპასუხე ამ Google review-ს თბილად, მოკლედ (max 60 სიტყვა), ჩვენი ბრენდის voice-ით:

[PASTE REVIEW]
```

### Prompt 5 — Negative Review Reply

```
უპასუხე უარყოფით review-ს — confirmation, ბოდიში, კონკრეტული გამოსავალი.
არ იყო defensive. მაქს. 80 სიტყვა.

[PASTE REVIEW]
```

### Prompt 6 — Google Business Profile Rewrite

```
გადააკეთე ჩვენი Google Business Profile-ის აღწერა SEO-ისთვის.
Keyword [city + service] 2-ჯერ, CTA ფინალში, max 750 სიმბოლო.

არსებული აღწერა:
[PASTE]
```

### Prompt 7 — Email Subject Lines

```
დაწერე 10 subject line ჩვენი newsletter-ისთვის [TOPIC]-ის შესახებ.
თითო max 50 სიმბოლო. 5 curiosity-based, 3 value-based, 2 urgency-based.
```

### Prompt 8 — Monthly Content Calendar

```
დაწერე 30 პოსტ-იდეა [MONTH]-ისთვის ჩვენი ბრენდისთვის.
დღე-დღეზე — თემა + hook + ფორმატი (Reel / carousel / static).
ქართული დღესასწაულები გათვალისწინე.
```

### Prompt 9 — Competitor Analysis

```
გავაანალიზე ეს კონკურენტი: [URL ან აღწერა].

დაუბრუნე:
- მათი value proposition
- სამიზნე აუდიტორია
- სუსტი წერტილი
- 1 აბზაცი — როგორ შეგვიძლია ჩვენ გამოვირჩეთ
```

### Prompt 10 — Hook Generator

```
დაწერე 10 hook (პოსტის პირველი ხაზი) [TOPIC]-ისთვის.
თითო 8-12 სიტყვა.
- 3 კითხვით
- 2 contrarian take-ით
- 2 პირადი ისტორიით
- 2 სტატისტიკით
- 1 funny ან cheeky-ით
```

---

## 💡 ერთი მთავარი რჩევა

Project არ არის „ერთხელ ჩაწერა და დაივიწყე" workflow.

**ყოველ თვეში გადახედე:**
- ცვალებს ბრენდი ტონს? — განაახლე Custom Instructions
- ახალი პროდუქტი დაამატე? — განაახლე product catalog
- ახალი customer review-ები დაგროვდა? — შეცვალე top 10

ეს 10 წუთიანი ყოველთვიური ჩარევა ინარჩუნებს, რომ Claude-ის output-ი დარჩეს ცოცხალი და ბრენდის ცვალებად რეალობასთან მორგებული.

---

<div align="center">

### უკან [მარკეტერების სექციაზე](./README.md)  ·  [მთავარი რეპო](../README.md)

</div>
