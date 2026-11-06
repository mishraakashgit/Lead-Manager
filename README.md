# Lead-Manager

Enquiry follow-up for small Instagram businesses (gifting, decor, jewellery, apparel, handmade).

**The problem being validated:** customers DM asking about price or availability, then go quiet, and the sale is lost because nobody followed up.

## What's here

| Path | What it is |
|---|---|
| [`prototype/index.html`](prototype/index.html) | Clickable prototype, one file, no backend. Daily view, pipeline, quick-add, one-tap follow-ups. |
| [`docs/research-log.md`](docs/research-log.md) | Seller conversations, decision rule, running tally |
| [`docs/outreach-and-demo.md`](docs/outreach-and-demo.md) | DM scripts and how to run a prototype demo with a seller |

## The prototype

Open `prototype/index.html` in any phone or desktop browser. It starts with 13 sample enquiries for a fictional shop ("Little Jhola Studio"), set up so the daily view shows **4 to follow up, 2 waiting for payment, 3 to ship**.

What it does:
- **Today:** what needs attention, with the ₹ value of enquiries waiting for a follow-up.
- **Quick-add (+):** name, Instagram handle, product, rough value. Shows how many seconds the entry took.
- **Pipeline:** Asked → Quoted → Waiting for payment → Paid → Shipped, plus Not interested.
- **Follow-up:** editable message for each stage. WhatsApp opens with the message typed in (`wa.me`). Instagram can't pre-fill a DM, so the message is copied and the chat opens (`ig.me/m/<handle>`). For sample customers the Instagram button only copies, so a demo never messages a real account.
- **Reminders:** a customer shows up in Follow up after 2 days of silence (1, 2, 3 or 5 days in Settings). Payment reminders after 1 day. "Tomorrow" snoozes.
- Changes are saved in the browser's local storage only. Settings → Reset brings the samples back.

### Put it online for demos (GitHub Pages)

1. Merge this branch into `main`.
2. Repo **Settings → Pages → Build and deployment → Deploy from a branch**, choose `main` and `/ (root)`.
3. The prototype will be at `https://<your-username>.github.io/Lead-Manager/prototype/`.

GitHub Pages on a private repository needs a paid GitHub plan. On the free plan, either make the repo public or use the shared artifact link.

## MVP scope (after validation)

1. Quick-add an enquiry in about 10 seconds
2. Simple pipeline
3. Follow-up reminders
4. One-tap follow-ups through WhatsApp or Instagram links. No WhatsApp Business API.
5. Daily view

Later: stock tracking, catalogue sharing, simple analytics.
