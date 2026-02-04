# DMI Portfolio Website (Static HTML/CSS)

This repository contains a clean, professional-looking **static portfolio website** used in **DevOps Micro Internship (DMI)** Week 1 to practice:
- Linux basics
- Nginx hosting
- Deployment proof / ownership
- Production-style checks

✅ Students deploy this website on an Ubuntu VM using Nginx and keep it live for 24 hours.

---

## Who is this for?
- DMI students (beginner → intermediate)
- Anyone learning how to host a static site with Nginx on Linux

---

## What you will build
A portfolio-style website hosted on:
- **Ubuntu VM**
- **Nginx**
- Accessible via: `http://<public-ip>`

---

## Mandatory Ownership Proof (DMI Rule)
Before you deploy, you MUST edit the footer and add your details:

Original:

```html
<p>Crafted with <span>cloud</span> excellence by Pravin Mishra</p>
```

Add this line (example):

```html
<p><strong>Deployed by:</strong> DMI Cohort 2 | Ashaye Adetomiwa | Group 2 | Week 4 | 04-02-2026</p>
```

```html
There is a footer requirement to make the date dynamic
To do this, I replaced the hardcoded date with a span tag that has a unique ID.
Then, I added the JavaScript by telling the browser to grab today's date and "inject" it into that span.
I added this script right before the closing </body> tag (usually at the very bottom of your index.html).

    <script>
    const dateElement = document.getElementById('deployDate');
    const now = new Date();

    const options = { day: '2-digit', month: 'short', year: 'numeric' };
    const formattedDate = now.toLocaleDateString('en-GB', options);

    dateElement.textContent = formattedDate;

    </script>

```

✅ This proof must be visible in your browser screenshot submission.