# Udyogini

**Fair work. Fair pay. Zero confusion.**

Udyogini is an AI-powered co-pilot for women's self-help groups (SHGs). It helps an SHG leader split a bulk order fairly among members, calculate materials and wastage, price the order correctly, and share the payment transparently.

Built by **Team SUDO** for **Tech4Bharat 2026**, Problem Statement 8.1 (Agentic AI): *Women's self-help groups lose orders and members' trust because fulfilment and pay are chaotic.*

> **Status:** Concept and design stage. The working prototype is being built. Screens in this repo are concept screens with sample data.

## The problem

From the organisers' problem statement 8.1:

- 10 to 15 members share each bulk order, with work divided verbally and tracked in notebooks
- Quality is checked only when output comes together
- Pay is split by estimate, and members underprice by 30 to 40% because material, labour and margin are never calculated
- Many members have low literacy

Source: Tech4Bharat 2026 problem statement 8.1.

## How it works

1. The customer types an order in plain words (for example, "200 jute bags in 10 days").
2. The AI lists the materials needed with a wastage allowance, and prices materials, labour and margin.
3. The SHG leader sees the price and a capacity check against the deadline, then accepts or declines.
4. The AI splits the work among members by skill, speed and availability, with the pay for each.
5. Each member receives a picture task with deadline and pay, in her language, with a "listen" button.
6. Members tick off finished work. The AI tracks progress and flags delays.
7. Members upload a batch photo against a quality checklist, and the leader inspects and approves.
8. The group approves the payout, every member sees her own record, and the customer is notified.

**Flow:** Order → AI estimate → Leader accepts → AI work split → Member tasks → Quality check → Group payout approval → Customer notified

## Key features

**Work, materials and pay**
- AI estimate of materials, wastage, labour and group margin
- Fair work split by skill, speed and availability, with a reason for each share
- Capacity check before the leader accepts, with a phased delivery suggestion
- Material stock tracking, low-stock alerts and reorder reminders
- Wastage recorded per order
- Price floor warning if a buyer negotiates below cost
- Pay calculated per member, with itemised deductions and reasons
- Group-approved payouts

**Made for real members**
- Picture tasks (photo, measurements, quantity)
- "Listen" button that reads tasks aloud
- Big tick button to mark work done
- English and local-language screens
- Shared-phone mode
- One-tap "I can't work this week", with automatic reassignment and a return plan
- Members see and hear their own earnings

**Quality and trust**
- Quality checklist with batch photos
- Early delay alerts to the customer
- Order status page
- Ratings after verified orders only
- Ranked groups with a reason shown for each rank, and a fair share of early orders for new groups
- Certificates for goals, based on tracked data
- Human approval at every key step

## Planned tech stack

- **Frontend:** mobile-friendly web app (HTML, CSS, JavaScript)
- **Backend:** Python
- **Database:** SQLite (prototype)
- **AI:** a large language model to understand orders and write plain-language explanations; Python code for pricing, wastage, work split and payout maths, so figures stay exact
- **Voice:** browser text-to-speech for the "listen" button

## What is simulated

Payments and outside systems are simulated and clearly labelled. All SHG, member and order data in this repo is sample data.

## Repository layout (planned)

```
docs/        deck, concept screens, briefing, field research notes
backend/     API, pricing, work split, wastage, payouts
frontend/    screens
data/        sample data
tests/       tests for pricing and split maths
```

## Team SUDO

| Name | Role |
|------|------|
| Likith Raj R | Team Leader |
| Dhruv K | Member |
| Jasleen Kaur | Member |
| Pentapati Hrudhay | Member |

## Roadmap

- Working prototype of the core flow, from order to verified payout
- Field research with real SHGs, with findings added to `docs/`
- Pooled raw-material buying
- Several groups sharing one large order
- Delivery records that help a group apply for a bank loan

## Licence

To be decided.
