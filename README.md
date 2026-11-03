# Archit Sharma | The environment I run

Interactive portfolio for Archit Sharma, Assistant System Administration Manager.
Live site: https://archit-rgb.github.io/archit_Sharma_portfolio

## What's on the site

- **Infrastructure map:** starts as an overview of six areas (Identity & Access, Cloud, Network, Email & Endpoints, Security, Automation) around an ops desk. Selecting an area reconfigures the whole page: the map re-centres on that area with its tools around it and the other areas along the bottom, the accent colour changes, and the detail panel updates.
- **Resolved tickets:** four written client commendations (by role only) plus incidents you handled (AD replication, Group Policy, DNS). Tickets related to the selected area are highlighted and the rest dimmed. The Customer Recognition Award and spot bonuses sit below.
- **Career:** a bar timeline of the three roles (Stigasoft/Infravision, Interra/VMware, Virtual Mind Infotech); roles that involved the selected area are highlighted.
- **Contact:** email and LinkedIn.

## Files

```
index.html   the whole site (HTML, CSS and JavaScript in one file)
README.md    this file
```

## Deploy on GitHub Pages

1. Put `index.html` and `README.md` in the root of your repository.
2. Commit and push to `main`.
3. In the repository, open **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. Open the live site after a minute or two.

## Editing

- The content for each map area is the `D` array near the bottom of `index.html`; area colours are the `COL` array. Which tickets and roles light up for each area is set by the `data-a` attributes (area numbers 0–5, in map order).
- Colours are CSS variables at the top of the `<style>` block.
- Animated packets on the map switch off automatically for visitors who prefer reduced motion.

## Notes

- Confirm with your employer and clients that publishing the feedback is fine.
- Never add credentials, internal hostnames or screenshots showing passwords to a public repository.

## Adding more feedback

Only add quotes clients actually wrote. To add one, copy a `<article class="tk" data-a="...">` block in `index.html`, paste their words in the `<q>` element, their role in `<p class="by">`, and set `data-a` to the area numbers it relates to (0 Identity, 1 Cloud, 2 Network, 3 Email & Endpoints, 4 Security, 5 Automation).
