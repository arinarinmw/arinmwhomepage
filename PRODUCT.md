# Product

<!-- impeccable:product-schema 1 -->

> Written 2026-10-16. The interview was answered from this session's history (the user said "you know the drill") instead of a live Q&A. Facts marked **[inferred]** were not confirmed line by line; correct them freely.

## Platform

web

## Users

- **Primary [inferred]:** event organizers and the people who book speakers and trainers: HR, L&D and OD practitioners, universities, communities. Situation: a colleague forwards the link ("send the web to the OD friend"); they scan quickly for topics, formats, proof, and how to get in touch. Job: decide whether to invite Arin, and for which session.
- **Secondary [inferred]:** students and course learners arriving from YouTube, Skilllane, Udemy or Instagram who want to learn from Arin or check her background. Visitors read Thai, English, or both.

## Product Purpose

arinmw.com is Arin Muadthong's personal speaker and trainer profile. It exists to get her invited to talk, train and run workshops, and to show the courses and credentials behind that work. Success **[inferred]**: an organizer emails her with the audience, purpose, topic, and date of an event.

## Positioning

**[inferred]** A speaker whose teaching comes from about 15 years of real delivery in IT consulting, banking and startups (IBM, PwC SEA Consulting, Krungsri Nimble, a co-founded startup), backed by counselor and career-coach certification, who turns complex work into clear, practical lessons in both Thai and English. Her own line: "Making complex work clearer. Turning ideas into practical next steps."

## Operating Context

- Static site in the GitHub repo `arinarinmw/arinmwhomepage`, live at arinmw.com.
- Visitors arrive from shared links and from Arin's channels (YouTube "nobuglife by Arin MW", Instagram, LINE, Medium, Linktree, Skilllane, Udemy).
- Contact is by email (`arin.arinmw@gmail.com`) with a short brief the organizer is asked to send.
- A one-page "Arin Muadthong Speaker Profile" exists in Canva as the document counterpart; the website's training topics follow it.

## Capabilities and Constraints

- Plain HTML, CSS and a little vanilla JavaScript; no build step. Keep it deployable by pushing files to GitHub.
- Homepage sections today: Speaking & Training Topics (expandable list: Design Thinking, Agile Experimentation, AI as an Enabler), Formats & Audiences, Arin in Action (3 YouTube highlights shown as cover images that load the player on click, 4 campus-visit photos), Professional Profile (3 courses, 7 roles, certifications, education), and a contact block.
- Bilingual EN/TH toggle: English default, choice remembered, `?lang=th` opens Thai. Every English text has its Thai pair in the HTML; both must be kept in step.
- `free.html`, `decode-work.html`, `download-free-example.html` and `download-free-workbook.html` are for Thai-speaking course students. They currently share `site.css` with the homepage and must keep working. **[inferred scope]** The redesign targets the homepage first; those pages stay as they are unless the user says otherwise.
- Decided copy facts (2026-10-17, by Arin): "nearly 15 years" of experience; the co-founded company is shown as Absolute Consulting; the topic is named "Agile Experimentation".

## Brand Commitments

- The Thai name อรินจ์ หมวดทอง is never translated; it sits with "Arin Muadthong".
- Thai course titles, video titles and talk titles stay exactly as published, in both languages.
- The YouTube channel name is "nobuglife by Arin MW".
- **[inferred]** Voice: plain, practical, warm; no hype. Thai copy is conversational.

## Evidence on Hand

- Photo: `Media/Profile final with circle.jpg`
- Campus-visit photos (web copies, metadata stripped): `Media/campus/` (4 files: KMITL x2, Chulalongkorn, Chandrakasem Rajabhat online session with a participant's name blurred)
- Course covers: `Media/courses/` (Decode Work, Business Analyst Essentials on Skilllane; Practical User Stories on Udemy)
- YouTube videos: `yoisX2AFEGE`, `woGTyKNZybU`, `nLcWvX9TeGc`
- Work experience (7 roles), certifications (IBM, iStrong counseling levels, IAP career coach), and education (M.S. Northeastern, B.Sc. Chulalongkorn)
- Not available, so do not invent: testimonials, organizer or client logos, press mentions, speaker fees, availability or booking calendar, and any video of a full stage talk (the videos are from her own channel).

## Product Principles

1. Make the organizer's decision easy: topics, formats, proof and contact should follow in one clear path.
2. Show, don't claim: real videos, photos and projects come before adjectives.
3. The site should do what the tagline promises: make complex things clearer.
4. Thai and English are equals; neither should read like a translation of the other.
5. One primary action: an email with a useful brief.

## Accessibility & Inclusion

- Thai script must stay legible: Thai-capable type, generous line height, no letter-spacing tricks.
- **[inferred]** Target WCAG AA. The current design fails it in places (accent text 3.9:1, muted text 3.4:1, footer button hover 3.5:1).
- The language toggle and the expandable topic list must work by keyboard and with screen readers; respect reduced motion.
- **[inferred]** Mobile first: many visitors arrive from LINE and Instagram on phones.
