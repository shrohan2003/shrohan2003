# Shanjidul Hasan Rohan

I am a **full-stack Software Engineer (Independent Contractor) at Staksa Limited and MediaStarboard**, working remotely from Dhaka, Bangladesh since October 2026. I build frontend interfaces with React and Vue, backend APIs with Node.js and Express, and browser automation with Python. I also built a CI/CD pipeline using Terraform.

I integrate ChatGPT, Codex, Claude, and Gemini into an efficient development workflow, using task-specific prompts and the right tool for each stage to streamline research, implementation, debugging, and testing.

**Education:** I studied Computer Science and Engineering at BRAC University.

## Open source

As of November 21, 2026, I have **9 merged upstream pull requests** across **icalevents, python-caldav, python-semver, and sktime**.

- **Released in python-semver 3.1.1** · I fixed version indexing for objects that implement Python’s integer index protocol. [PR #508](https://github.com/python-semver/python-semver/pull/508) · [Release notes](https://github.com/python-semver/python-semver/discussions/510)
- **Merged** · I fixed a numerical stability issue in `PolynomialTrendForecaster` by rescaling timestamps before fitting the trend. The fitted coefficients retain their original time units. [sktime #11472](https://github.com/sktime/sktime/pull/11472)
- **Merged** · I added test cases that run without optional dependencies, allowing sktime to re-enable a parameter coverage test for 14 estimators. [sktime #11624](https://github.com/sktime/sktime/pull/11624)
- **Merged** · I removed obsolete test skips for eight estimators so those tests now run in the suite. [sktime #11562](https://github.com/sktime/sktime/pull/11562)
- **Open as of November 7, 2026** · I proposed a fix for `OnlineEnsembleForecaster` so updating a forecast leaves the caller’s ensemble object intact and fitting the model again starts with fresh weights. [sktime #11621](https://github.com/sktime/sktime/pull/11621)

### Calendar software

Both python-caldav fixes and three icalevents fixes have merged. Additional calendar fixes remain under review.

- **ical.js** · I proposed fixes for reading contact photos from vCards, importing files with multiple calendars, and converting dates before a time zone’s first transition or with years below 1000. [vCard photos](https://github.com/kewisch/ical.js/pull/1080) · [Calendar streams](https://github.com/kewisch/ical.js/pull/1081) · [Time zone offsets](https://github.com/kewisch/ical.js/pull/1082) · [Early years](https://github.com/kewisch/ical.js/pull/1083)
- **python-caldav** · One patch keeps an alarm’s ID from being mistaken for its parent event’s ID. Another reports when a server rejects an individual property update. [Event IDs](https://github.com/python-caldav/caldav/pull/858) · [Property updates](https://github.com/python-caldav/caldav/pull/859)
- **icalevents · Merged** · I prevented a deadlock when multiple asynchronous calendar requests share a key, fixed imports with repeated categories, and included ongoing recurring events in narrow searches. [Async requests #189](https://github.com/eigenmannmartin/icalevents/pull/189) · [Categories #182](https://github.com/eigenmannmartin/icalevents/pull/182) · [Recurring events #183](https://github.com/eigenmannmartin/icalevents/pull/183)
- **icalevents · Under review** · Fixes for exclusive all-day end dates, exact recurrence exclusions, and occurrences moved outside the query window. [#184](https://github.com/eigenmannmartin/icalevents/pull/184) · [#185](https://github.com/eigenmannmartin/icalevents/pull/185) · [#190](https://github.com/eigenmannmartin/icalevents/pull/190)

## Selected projects

- **MediaStarboard · CI/CD & cloud infrastructure** — In my current role at MediaStarboard, I work on CI/CD and cloud infrastructure using GitHub Actions, Terraform, and AWS, including automated checks and beta deployments for the frontend and backend. My work also covered deployment safeguards and operational documentation.

- **Calendar Recurrence Lab** lets you cancel meetings and compare the expected schedule with results from two pinned parser revisions across all 64 cancellation patterns. [Live demo](https://shrohan2003.github.io/calendar-recurrence-lab/) · [Source](https://github.com/shrohan2003/calendar-recurrence-lab)
- **Calendar UID Map** compares local calendar exports, distinguishes reminders from their parent events, and flags repeated master records. [Source and example](https://github.com/shrohan2003/calendar-uid-map)

- **Collaborative Notes** lets owners share individual notes with readers or editors. The Vue interface calls an Express API, and PostgreSQL stores the notes and access permissions. [Repository](https://github.com/shrohan2003/collaborative-notes-app)
- **BRACU Bazaar** is a student marketplace I worked on as part of a BRAC University software engineering team. The group built the catalog, order flows, and messaging with React, Express, and MongoDB. [Group repository](https://github.com/Fazlul105/BRACU-Bazaar)

## Skills

- **Python and data** · HTML parsing with Beautiful Soup, browser automation, pytest, and time-series forecasting. My academic work includes pandas, NumPy, and scikit-learn.
- **Web development** · JavaScript, TypeScript, Vue, React, and REST APIs with Node.js and Express.
- **Databases and tools** · SQL, PostgreSQL, Cloudflare D1, Cloudflare Workers, and Git.

[Portfolio](https://shanjidul-rohan.netlify.app/) · [LinkedIn](https://www.linkedin.com/in/shanjidul-hasan-rohan-b96189335/) · [Email](mailto:shanjidul.hasan.rohan@g.bracu.ac.bd)
