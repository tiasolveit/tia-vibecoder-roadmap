# 🔴 Track 3: Vibecoder Pro

**Goal:** Make it solid, safe, and scalable.

Now that the product works and people use it, the cost of being wrong goes up.
This track is where you stop losing money and data to preventable problems.

Order matters more here than in the other tracks. Do security before payments.

---

## 1. 🔐 الأمان

Audit what you expose. No secrets in client-side code, no open endpoints, no
unvalidated input, no missing auth checks on private data.

Enable rate limiting on auth endpoints. Add MFA on any admin account. Turn on
CORS, CSP, and HTTPS everywhere including the API.

**Done when:** You have run an automated dependency scan and you have manually
checked every route that reads user data.

---

## 2. 📜 القانوني والخصوصية

Add the boring pages: privacy policy, terms of service, and a real data
deletion path. If you collect email or payment data, say so plainly.

Know where your data lives and who can reach it. If you use a third-party
service that can see user data, name it in the policy.

**Done when:** A user can read the policy, understand what you store, and
delete their account and their data without emailing you.

---

## 3. 💳 المدفوعات

Handle payments the boring way: server-side price calculation, webhook
verification on every event, and idempotency on every charge.

Never trust a price the client sends. Handle the failed payment and the
cancelled subscription, not just the happy path.

**Done when:** You can grant and revoke access automatically from payment
events, and a replayed webhook does not double-charge anyone.

---

## 4. ☁️ النسخ الاحتياطي

Automate backups of the database, and restore one on purpose. A backup you
never tested is a rumor.

Add rate limits and query monitoring too. One loop with no limit is the most
common way a small product dies.

**Done when:** You have restored a full backup into a clean environment and
confirmed the data was correct.

---

## 5. 📈 التوسع والأداء

Watch what the app actually does. Slow queries and N+1 calls before they
become outages.

Add caching where it measurably helps, not everywhere. Cache invalidation is
harder than the slow query was.

**Done when:** You have a real load number under real traffic, and you know
which query to fix first if it doubles.

---

## 6. 🔌 التكاملات

Connect the tools you depend on, and make failures survivable. Sync is
eventually consistent, so design for that from the start.

Webhooks should verify signatures, retry on failure, and be safe to receive
twice.

**Done when:** One third-party failure has been simulated and your app degrades
instead of breaking.

---

## 7. 🐛 تتبع الأخطاء

Add error tracking and source maps before the first outage, because you cannot
debug what you cannot see. Capture user id, route, and request context.

Then alert on the errors that actually matter. An alert for every error is an
alert you will mute.

**Done when:** You have received a real alert from a real error and fixed it
before a user reported it.

---

## 8. 🧾 التوثيق

Write the doc you wished you had on day one. Setup, environment variables,
deploy steps, architecture in one page.

Also write an architecture note that says what you decided against and why.
That is what stops future you from rewriting the same mistake.

**Done when:** Someone who is not you can clone, run, and deploy the project
from your documentation alone.

---

## 9. 🧯 إدارة المخاطر

List what could hurt you: data loss, provider outage, payment dispute, a bug
that costs money, a key you rotate at the wrong time.

For each one, write the response. Then buy the cheap insurance. A monitoring
plan and a daily database backup cost almost nothing and cover most of the list.

**Done when:** You have a one-page risk list, and the top two risks have a
tested mitigation.

---

## What's next

You have shipped the framework. The road is now about what only you can do:
finding the specific problem you understand better than anyone, and staying on
it after it stops being fun.

- [Back to README](../README.md)
- [Prompt basics](00-prompt-basics.md)