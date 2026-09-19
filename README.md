# Shanjidul Hasan Rohan

Final-semester Computer Science and Engineering student at BRAC University. Python is my main programming language, and I also work with backend, frontend and full-stack web applications.

I am interested in junior software engineering, Python development and backend roles.

## Technical focus

- **Python:** browser automation, HTML parsing, data processing and object-oriented programming.
- **Web:** JavaScript, TypeScript, Vue, React, Express and REST APIs.
- **Data:** PostgreSQL, Cloudflare D1 and relational data modeling.
- **Tools:** Git, GitHub, pytest and Cloudflare Workers.

My academic work also includes machine-learning notebooks using pandas, NumPy and scikit-learn.

## Problem solving

I have solved 70+ coding problems through LeetCode/NeetCode practice.

## Selected projects

### [11 Brothers FC](https://github.com/shrohan2003/11-brothers-fc-case-study)

**My first paid real-world client project, built individually.** I developed a web platform for a football club to bring public club information, player accounts, registrations and administration into one place.

I built the TypeScript and React interface, server-side application workflows and database integration. Visitors can browse club information, players, matches and events. Players can create accounts and use a personal dashboard. Staff pages support club content, registrations and manual payment review.

**How the parts connect:** React displays the pages and forms. Server routes run on Cloudflare Workers using Vinext. Those routes read or save records in Cloudflare D1, a SQL database, while Cloudinary handles media storage. The browser sends requests to the server; it does not connect directly to the database.

**Example process:** A player opens a registration form and submits it. The server reads the login session, checks the relevant access and registration rules, and saves an accepted registration in D1. The interface displays the result returned by the server. Payment proof follows a separate staff-review workflow; it is not an automatic card-payment gateway.

**Stack:** TypeScript, React, Vinext, Tailwind CSS, Cloudflare Workers, D1, Drizzle and Cloudinary.

The linked case study includes real local demonstration screenshots. Client source remains private. Public pages, player account flows and local checks were tested; administrative and external-service workflows still need broader validation, and authentication hardening remains a known task.

### [Collaborative Notes](https://github.com/shrohan2003/collaborative-notes-app)

A full-stack notes project where registered users create private notes, search them and share selected notes with other users. The owner controls sharing. An editor can change the note, while a viewer can only read it.

**How the parts connect:** Vue provides the screens. It sends HTTP requests to an Express API, which uses PostgreSQL to store users, notes and sharing permissions. The backend is split into controllers that receive requests, services that check rules, and repositories that run SQL queries.

**Example process:** After login, the frontend stores a JWT and includes it with protected requests. When a user saves a note, Express checks the token, validates the title and content, and uses the authenticated user as the owner. A repository saves the record in PostgreSQL. The API returns JSON, and Vue shows the saved note. When another user opens a shared note, the backend checks that user's access before returning it.

**Stack:** JavaScript, Vue 3, Node.js, Express, PostgreSQL, JWT and bcryptjs.

This is permission-based sharing, not simultaneous live typing. The repository includes source, setup instructions, screenshots and tests. The description explains the application's implementation; it does not claim sole authorship or an unconfirmed division of work.

### [EVENTIM Event Data Scraper](https://github.com/shrohan2003/eventim-event-scraper)

**My individual Python project.** I built a tool that turns event-page content into structured JSON, making information such as the event name, venue, date and ticket categories easier to inspect and process.

I separated browser capture, HTML parsing, value cleanup and output into different Python modules. Dataclasses hold the result in a consistent structure, and offline tests check the parsing and error-handling behavior.

**How the parts connect:** This is a command-line application, so it does not have a separate web frontend, web backend or database. The command-line entry point passes an event URL or saved HTML file to the scraper. The browser component obtains page HTML when live access is available. The parser extracts fields, normalization helpers clean values such as prices, and the result is written to a JSON file.

**Example process:** Run the command with a saved page. The scraper reads the HTML, finds event and ticket information, creates structured Python objects and exports JSON. The same parser can be tested with fixtures without opening a live browser. Live access may fail if the website changes or restricts access; individual-seat availability is not guaranteed.

**Stack:** Python, Playwright, BeautifulSoup, dataclasses and pytest.

The repository remains private, so its link works only for people with access. The eight tests in this repository are separate from the fourteen tests in the newer local V3 implementation.

### [BRACU Bazaar](https://github.com/Fazlul105/BRACU-Bazaar)

**BRAC University CSE470 Software Engineering group project.** I participated as a team member in a student marketplace project. The group application includes product listings, account flows, orders, reviews and messaging. My exact responsibilities are not specified here because the available Git history does not establish the work split.

**How the parts connect:** React displays the marketplace. It requests data from an Express API, and the backend uses Mongoose to read or write MongoDB documents. The frontend is hosted on Netlify, with API requests forwarded to the backend on Render. Account-related code uses bcrypt password hashing and JWTs.

**Example process:** A visitor opens the catalog. React requests product data from the API. Express reads product records through Mongoose, returns JSON, and React displays the listings. Account and order routes are present in the source, but their protected live workflows were not tested during this review.

**Stack:** JavaScript, React, Vite, Tailwind CSS, Express, MongoDB and Mongoose.

[Live demo](https://bracubazaar.netlify.app/) | [Original group repository](https://github.com/Fazlul105/BRACU-Bazaar)

## Contact

[Email](mailto:shanjidul.hasan.rohan@g.bracu.ac.bd)

[LinkedIn](https://www.linkedin.com/in/shanjidul-hasan-rohan-b96189335/) | [GitHub](https://github.com/shrohan2003)
