---
title: "Claude Code Skills — ქართული გზამკვლევი"
layout: default
parent: "AI და კოდირება"
nav_order: 4
permalink: /ai-coding/claude-skills-guide/
description: "Battle-tested Claude Code skills — 6 slash command პროფესიული AI workflow-სთვის. ქართული გზამკვლევი + install instructions."
---

# 🛠 Claude Code Skills — ქართული გზამკვლევი

ეს გვერდი ქართულად ამხსნელია **Claude Code Skills** კოლექციისა, რომელიც [@alexknowshtml](https://github.com/alexknowshtml)-მა შექმნა და ღია კოდად გამოაქვეყნა GitHub-ზე.

> **ორიგინალი რეპო:** [github.com/alexknowshtml/claude-skills](https://github.com/alexknowshtml/claude-skills)
> **ავტორი:** [@alexknowshtml](https://github.com/alexknowshtml)
> **აღმოაჩინა:** [Tom Dörr (@tom_doerr)](https://x.com/tom_doerr) — X-ზე ვირუსული პოსტი
> **ლიცენზია:** იხილე ორიგინალ რეპოში

---

## 🎯 რა არის Claude Code Skill?

Skill — ეს არის markdown ფაილი, რომელიც Claude Code-ში გადაიქცევა **slash command-ად** (მაგ. `/reflect`). შენ ერთხელ ჩასვამ ფაილს — შემდეგ შენი ნებისმიერ Claude Code session-ში გამოიყენებ `/name`-ით.

ეს კონკრეტული კოლექცია არის **"battle-tested"** — ცოცხალ production workflow-ში გამოცდილი, არა experimental.

---

## 📚 6 Skill — რას აკეთებს თითო

### 1️⃣ `/reflect` — სესიის რეტროსპექტივა

რას აკეთებს:
- სკანავს მიმდინარე session-ს
- აღმოაჩენს რა friction იყო და რა ისწავლე
- **ავტომატურად ნერგავს quick wins-ს** (პატარა გასწორებები რომელიც დროს დაზოგავს)

როდის გამოიყენო:
- სესიის ბოლოს, სანამ workspace-ს დახურავ
- როცა გრძნობ რომ რამე გადაიხსნა, მაგრამ კონკრეტი ფორმულირება არ გაქვს

---

### 2️⃣ `/pause` — Session State-ის შენახვა

რას აკეთებს:
- ინახავს session-ის მიმდინარე state-ს
- ქმნის **return prompt-ს** — მერე გასაგრძელებლად მზად
- აქვს ორი mode: quick (სწრაფი) და full (სრული)

როდის გამოიყენო:
- როცა session-ი დიდია და context-ი იწურება
- როცა გინდა შესვენება, მაგრამ კონტექსტი არ დაკარგო

---

### 3️⃣ `/upskill` — Skills-ის განახლება

რას აკეთებს:
- სკანავს session-ს
- აღმოაჩენს **stale skills** (მოძველებული, აღარარელევანტური)
- გვთავაზობს **ახალ skill candidates** (workflow-დან რომელიც skill-ად ღირს)
- ავტომატურად დანერგავს განახლებებს

როდის გამოიყენო:
- კვირაში ერთხელ — workflow-ის ჰიგიენისთვის
- როცა შენი skills-ის ბიბლიოთეკა იზრდება და უნდა გადახედო

---

### 4️⃣ `/create-skill` — Session-დან Skill-ის შექმნა

რას აკეთებს:
- იღებს მიმდინარე session-ს
- გადის **research + planning + approval flow-ს**
- ქმნის მზა **markdown skill ფაილს** რომელიც შემდეგი სესიისთვის გამოგადგება

როდის გამოიყენო:
- როცა workflow აღმოაჩინე და გინდა რომ მერე გაიმეორო
- პროცესის სტანდარტიზაცია, რომელიც ხშირად მეორდება

---

### 5️⃣ `/pretty-page` — Markdown → ლამაზი HTML Page

რას აკეთებს:
- იღებს ნებისმიერ markdown-ს → ქმნის **სტილიზებულ HTML გვერდს**
- ატვირთავს **S3-compatible storage-ში**
- მოგცემს public URL-ს გასაზიარებლად

როდის გამოიყენო:
- როცა გინდა markdown-ი (notes, retrospective, document) კოლეგას გაუგზავნო
- როცა web link-ი გჭირდება, არა attachment

---

### 6️⃣ `/teach` — Socratic Teaching Loop

რას აკეთებს:
- იღებს session-ს → ამოაჩენს **quiz topics**
- სვამს კითხვებს თვითონ თავის თავს
- **mastery item-by-item** — არ ამთავრებს სანამ ყველა საკითხს არ დაეუფლე

როდის გამოიყენო:
- როცა რთული თემა გავიგე და გინდა მტკიცე გათავისება
- სასწავლო კონსოლიდაცია — ცოდნა მუდმივად რომ შემორჩეს

---

## 🚀 დაყენების ნაბიჯები

### ნაბიჯი 1 — Clone რეპო

```bash
git clone https://github.com/alexknowshtml/claude-skills.git
```

### ნაბიჯი 2 — Skill-ის კოპირება

ორი ვარიანტი არსებობს:

**ვარიანტი A (რეკომენდებული):**
```bash
cp -r reflect ~/.claude/skills/reflect
```

**ვარიანტი B (უფრო მარტივი):**
```bash
cp reflect/SKILL.md ~/.claude/commands/reflect.md
```

გაიმეორე ყველა skill-სთვის: `pause`, `upskill`, `create-skill`, `pretty-page`, `teach`.

### ნაბიჯი 3 — Customize

ყველა SKILL.md-ში არის **placeholders** `<angle-brackets>`-ით აღნიშნული. სანამ გამოიყენებ, ჩაანაცვლე შენი მონაცემებით (paths, config).

### ნაბიჯი 4 — გამოყენება

ახალ Claude Code session-ში დაუწერე `/reflect` (ან რომელიც აარჩიე) — შესაბამისი skill ავტომატურად ჩაირთვება.

---

## ⚙️ Project-ვს Global Skills

| Scope | Path | როდის გამოიყენო |
|-------|------|----------------|
| **Project-ი** | `.claude/skills/` | მხოლოდ კონკრეტული პროექტისთვის |
| **Global** | `~/.claude/skills/` | ყველა Claude Code session-ში ხელმისაწვდომი |

**რეკომენდაცია:** **Global** scope ჯობია — ერთხელ დააყენე, ყველგან მუშაობს.

---

## 🤝 Credits

ეს გვერდი ქართული ადაპტაციაა — სრული credit ორიგინალ ავტორებს:

- **ავტორი:** [@alexknowshtml](https://github.com/alexknowshtml) — Claude Skills-ის შემქმნელი
- **აღმოაჩინა:** [Tom Dörr (@tom_doerr)](https://x.com/tom_doerr) — X-ზე ვირუსული პოსტი
- **ქართული ადაპტაცია:** [Tamar Khatiashvili](https://github.com/TakoTechie1)

თუ მოგწონს ეს კოლექცია — გადადი ორიგინალ რეპოზე და დათანე ⭐ Star: [github.com/alexknowshtml/claude-skills](https://github.com/alexknowshtml/claude-skills)

---

## 📚 დამატებითი რესურსები

- 🔗 **ორიგინალი რეპო:** [github.com/alexknowshtml/claude-skills](https://github.com/alexknowshtml/claude-skills)
- 🔗 **Tom Dörr-ის ვირუსული პოსტი:** [@tom_doerr X-ზე](https://x.com/tom_doerr)
- 🔗 **Claude Code დოკუმენტაცია:** [docs.claude.com/en/docs/claude-code](https://docs.claude.com/en/docs/claude-code)
- 🔗 **Claude Code Plugins:** [Claude Code Plugins](https://docs.claude.com/en/docs/claude-code/plugins)

---

ცადე ეს skills და მითხარი რომელი მუშაობს შენთვის ყველაზე კარგად 🤍
