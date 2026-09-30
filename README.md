# Worth The Calories

Coming-soon page and waitlist for an app that turns a photo of a dish into a calorie range, the ingredients worth knowing about, and a verdict. `index.html` is the one-screen teaser (hook, coming soon, email). `full.html` is the full page for later, unlinked. Painting, share card (`og.jpg`) and the Story poster (`poster-story.jpg`) live in `assets/`.

Signups: the form POSTs to a Google Apps Script web app (project "WTC waitlist" on yuvrajangad.s@gmail.com, bound to the sheet of the same name) that appends a time and email row. The script treats the 302 Apps Script always returns as success and does not follow it, because the redirect target 404s now and then while the row has already landed. Editing the script needs Deploy > Manage deployments > edit > new version to go live; the URL stays. A brand new deployment gets a new URL and the `action` attribute has to follow.

Deploy: push to GitHub, then Settings > Pages > deploy from the main branch, root folder, custom domain worththecalories.fit (the `CNAME` file), enforce HTTPS. DNS at Namecheap already points there.

Before sending any email to the list: it needs a working unsubscribe and a postal address (CAN-SPAM), and the page still needs a privacy note naming who runs it, a contact email and how long signups are kept.

Every URL the page cites (claims, evidence, nutrition data, image) is listed in `.notes/sources.md`.
