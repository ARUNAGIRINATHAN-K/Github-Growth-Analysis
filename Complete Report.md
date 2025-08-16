Here’s a concise, data-driven report on what drives GitHub follower growth (and whom to follow), with an emphasis on the role of stars and contributions. I’ve included two quick charts to anchor the correlations reported in the literature.

# 1) Introduction

On GitHub, **followers** signal personal influence and reach; **following** shapes your feed and collaboration surface; **stars** are an easy, public signal of interest; and **contributions** (issues, PRs, commits, reviews) are the substance of value creation. In practice, followers grow when developers (a) repeatedly create visible value and (b) get discovered—often through starred repos, cross-project contributions, social shares, and mentions in trending lists or newsletters. Research also shows “popular users” can **pull their followers** toward new projects they star/fork/contribute to, reinforcing visibility loops. ([Dr Kelly Blincoe][1])

# 2) Correlation analysis: stars ↔ followers

**Takeaway:** Stars correlate with attention and discovery, but they are an imperfect proxy for real adoption—and they’re not immune to manipulation.

* A 2024 study of web-source libraries finds that the **correlation between stars and package downloads is weak** (r ≈ 0.14 for JavaScript, ≈ 0.47 for PHP). Yet stars correlate **moderately** with **detected deployments** (r ≈ 0.61–0.63). This supports the idea that stars reflect visibility/interest more than usage, but aren’t meaningless. *(Chart below reproduces the reported r values.)* ([MADWeb 2025][2])
* Qualitative analyses of star growth (e.g., Appsmith’s 4,500 stargazers in nine months; CockroachDB’s “Stargazers” tooling) show stars track **who is noticing you** (geos, referrers, timing) and can help teams learn where attention comes from—even if the download/use signal is noisy. ([Appsmith][3], [Cockroach Labs][4])
* Caveat: There’s a **black market** for fake stars/followers; independent work documents millions of suspected fake stars and campaigns that artificially spike popularity. Treat raw star counts and sudden spikes with caution. ([WIRED][5], [arXiv][6])

(See the two small correlation charts above for the reported r values.) ([MADWeb 2025][2])

# 3) Impact of contributions on follower growth

**Active, visible contribution** is one of the most reliable ways to gain followers:

* **Influence cascades:** When “popular users” interact with projects (star/fork/contribute), their followers frequently discover and then engage with those projects—implying that **your contributions in visible repos** can broadcast you to wider audiences. ([Dr Kelly Blincoe][1])
* **Behavioral evidence:** Studies on following/contributions suggest **receiving new followers** is associated with **increased contribution levels**, especially for unaffiliated individuals—consistent with social feedback loops (attention → motivation → more activity). ([PolyU Institutional Research Archive][7])
* **Health vs. hype:** Community analyses recommend looking beyond stars to **commit velocity, issues, PRs, and contributor counts** as better markers of authentic engagement—the very actions that also make contributors more discoverable and credible to potential followers. ([OpenSauced][8])

**Key metrics to watch for follower lift from contributions**

* # of PRs opened/merged in high-visibility repos
* # of issues triaged/resolved; response latency
* % of contributions that get referenced (release notes, changelogs)
* Cross-project footprint (distinct orgs you’ve contributed to)
* Mentions in maintainers’ READMEs, release notes, or social posts

# 4) Case studies

**996.ICU (social movement repo):**

* Catapulted to >200k stars within days/weeks in 2019, becoming one of GitHub’s most-starred repos. The org account today shows \~8.5k followers—illustrating that **mass visibility events** (press, HN/Reddit, social shares) can produce both star and follower spikes. ([Made in China Journal][9], [Hacker News][10], [The Engineering Manager][11], [GitHub][12])

**Sindre Sorhus (developer brand via many repos, e.g., “awesome”):**

* Maintains widely followed repos (e.g., *awesome*, \~392k stars) and has \~74k personal followers—consistent with the idea that **sustained contributions across many useful repos** convert broad star-level attention into durable personal following. ([GitHub][13])

**Appsmith (product-led OSS):**

* Their internal analysis of early stargazers found a **weak positive relation** between stargazers’ follower counts and their commit activity—again, stars signal attention clusters, and ongoing contribution/usage deepens community ties. ([Appsmith][3])

**CockroachDB (analytics on stars):**

* Built tooling to analyze stargazers over time, surfacing where attention originates (e.g., referrers, regions), which can guide targeted community outreach that in turn impacts star and follower trajectories. ([Cockroach Labs][4])

# 5) Best practices to increase followers (and follow smartly)

**A. Ship value where people already look**

* Contribute PRs/issues to **high-visibility repos** (popular frameworks, tooling, “awesome” lists, DevEx utilities). Your handle gets exposure in PR threads, release notes, and dependency graphs. ([Dr Kelly Blincoe][1])
* Publish **use-once, star-often** utilities: CLIs, templates, examples that remove friction for common tasks. (These frequently get starred, then shared in newsletters.)

**B. Make stars work as a discovery funnel (but guard integrity)**

* Optimize **README first screen**: a crisp value prop, quickstart, badges (CI, coverage), and a “What it looks like” gif.
* Add **referrer beacons** (UTM links in docs/blogs) and track star bursts by source—replicate channels that work. ([Cockroach Labs][4])
* Avoid inorganic tactics; **fake-star spikes** can harm trust. Use tools/heuristics (e.g., StarGuard) to **monitor suspicious star bursts** in your own repos and competitors. ([GitHub][14], [arXiv][6])

**C. Turn contributions into lasting followers**

* Be **responsive**: fast triage, helpful reviews, and constructive code comments. Many “How I got 1k stars” retros point to **maintainer responsiveness** as a growth lever. ([Eke][15])
* Create **contributor-friendly scaffolding**: good first issues, CONTRIBUTING.md, CI that runs in forks, reproducible dev containers.
* **Narrate your work**: changelogs, release threads, short demos on X/LinkedIn/Reddit. Popular users can bring their followers; your posts can, too. ([Dr Kelly Blincoe][1])

**D. Cross-ecosystem presence**

* Write short posts about your repo on Dev.to/Medium, share in relevant community discords/slacks, and pitch newsletter maintainers. These channels drive stargazers who then discover *you*. ([Medium][16])

**E. Who to follow (strategic following)**

* Follow maintainers in your domain; comment constructively on issues/PRs. This improves your **feed quality** (discovery) and your **name recognition** within that niche—both precursors to follower growth. ([Dr Kelly Blincoe][1])

# 6) Conclusion

* **Stars** are a strong *visibility* signal but an imperfect adoption proxy; correlations with **downloads** are weak, while correlations with **deployments** are moderate. Think of stars as top-of-funnel attention that can lead to followers. ([MADWeb 2025][2])
* **Contributions**—especially in visible repos—are the most consistent driver of follower growth because they place your work in front of already-engaged audiences and trigger influence cascades. ([Dr Kelly Blincoe][1], [PolyU Institutional Research Archive][7])
* Sustainable growth blends **useful artifacts** (reliable repos), **visible activity** (PRs, issues, reviews), and **trust** (no fake-star games). Treat stars as a discovery engine; treat contributions as the conversion mechanism from attention → adoption → followers.

If you’d like, I can tailor a bite-size plan for your profile (repos to target, weekly contribution cadence, and lightweight analytics to track star/referrer → follower conversion).

[1]: https://kblincoe.github.io/publications/2015_IST_Blincoe.pdf?utm_source=chatgpt.com "[PDF] Following, Affiliation Influence and Leadership on GitHub"
[2]: https://madweb.work/papers/2024/madweb24-koch.pdf?utm_source=chatgpt.com "[PDF] An Analysis of GitHub Stars as an Importance Metric for Web Source ..."
[3]: https://www.appsmith.com/blog/in-9-months-4500-people-starred-appsmith-on-github-what-do-we-know-about-them?utm_source=chatgpt.com "In 9 Months, 4500 People Starred Appsmith on Github. What Do We ..."
[4]: https://www.cockroachlabs.com/blog/what-can-we-learn-from-our-github-stars/?utm_source=chatgpt.com "Stargazers: A tool for analyzing your GitHub stars - CockroachDB"
[5]: https://www.wired.com/story/github-stars-black-market-coders-cheat?utm_source=chatgpt.com "The GitHub Black Market That Helps Coders Cheat the Popularity Contest"
[6]: https://arxiv.org/html/2412.13459v1?utm_source=chatgpt.com "4.5 Million (Suspected) Fake \faStar Stars in GitHub - arXiv"
[7]: https://ira.lib.polyu.edu.hk/bitstream/10397/97049/1/Mei_Effect_Following_Contributions.pdf?utm_source=chatgpt.com "[PDF] The Effect of “Following” on Contributions to Open Source ..."
[8]: https://opensauced.pizza/blog/growth-hacking-killed-github-stars?utm_source=chatgpt.com "Growth Hacking Killed GitHub Stars - Open Sauced"
[9]: https://madeinchinajournal.com/2019/06/18/the-996-icu-movement-in-china-changing-employment-relations-and-labour-agency-in-the-tech-industry/?utm_source=chatgpt.com "The 996.ICU Movement in China: Changing Employment Relations ..."
[10]: https://news.ycombinator.com/item?id=19498179&utm_source=chatgpt.com "996.icu, Chinese programmers against working overtime gathering ..."
[11]: https://www.theengineeringmanager.com/current-affairs/the-rebellion-against-chinas-996-culture/?utm_source=chatgpt.com "The Rebellion Against China's 996 Culture"
[12]: https://github.com/996icu?utm_source=chatgpt.com "996icu - GitHub"
[13]: https://github.com/sindresorhus/awesome?utm_source=chatgpt.com "Awesome lists about all kinds of interesting topics - GitHub"
[14]: https://github.com/m-ahmed-elbeskeri/Starguard?utm_source=chatgpt.com "m-ahmed-elbeskeri/Starguard - GitHub"
[15]: https://eke.hashnode.dev/how-my-open-source-project-got-1000-stars-on-github-in-4-months?utm_source=chatgpt.com "How my open source project got 1000 stars on GitHub in 4 months"
[16]: https://medium.com/neural-engineer/tracking-github-repository-growth-analyzing-stars-and-forks-timelines-2ef343a0da44?utm_source=chatgpt.com "Tracking GitHub Repository Growth: Analyzing Stars and Forks ..."
