🎧 UX Case Study — Improving Music Discovery in Spotify Desktop

By Adrien Vieilledent, Charlene Billot-Mornet, and Frédéric Bourouliou

⸻

🏁 Overview

This UX case study was part of the project [C#25] Spe – Web Stack Programming 2025 v2, where our challenge was to think like designers and improve the Spotify Desktop experience.

The goal:

How can we help users find music more easily?

We worked from predefined personas provided by the UX Research team, each representing a specific Spotify user type.
Our assigned persona was Michelle, a nurse practitioner and mother of four, who struggles to explore new music because Spotify’s recommendations are biased by her kids’ listening habits.

⸻

🎯 Problem Statement

Spotify’s recommendation system mainly reflects the tastes of the most active listeners in a shared account — usually the children.
Michelle cannot afford a separate account, yet she wants a personal music experience that reflects her mood and needs, without constant manual filtering.

Our goal was to design a low-effort, personalized, and family-friendly experience inside the Spotify Desktop app.

⸻

👥 User & Audience
	•	Primary user: Michelle (42, nurse practitioner, mother of four).
	•	Needs: quick access, low cognitive load, tailored discovery.
	•	Secondary users: her children (ages 5–12), who need a simplified, safe, and playful experience.

⸻

🧩 Roles & Responsibilities
	•	Team size: 3 designers
	•	My role: UX analysis, user flow design (Mermaid), and desktop mockups (Figma).
	•	Tools: Figma, Miro, GitHub (repository documentation), Mermaid, Markdown.

⸻

⏱ Scope & Constraints
	•	Platform: Spotify Desktop App
	•	Persona and initial research provided by the school’s UX Research team
	•	Timeframe: 2 weeks
	•	Deliverables: research synthesis, user flow, Figma prototype, usability validation

⸻

🧠 Process & What We Did

1. Understanding the Challenge

“How can Spotify help Michelle find new music for herself, even when sharing her account with her family?”

2. Research & Discovery
	•	We analyzed the persona’s journey: moments of fatigue, family context, multitasking.
	•	Key pain points:
	•	Overloaded recommendations
	•	Confusing interface when tired
	•	Lack of personal control in a shared account

3. Ideation (Sketch & Brainstorm)

We explored several ideas during whiteboarding sessions:

#	Team’s ideas
1	Mood bubbles: morning / noon / evening quick playlists
2	“Search for Me” button for AI-powered discovery
3	Smart onboarding quiz (3 quick questions)
4	Family profile switcher (adult / child)
5	Reduced recommendations from 10 → 5
6	Enhanced sidebar filters (adult / child / both)


⸻

4. Design Decisions

We decided to combine the most impactful ideas:
	•	Profile selection → Adult or Child entry point
	•	Mood bubbles for low-effort discovery moments
	•	“Search for Me” → one-click tailored recommendations
	•	Reduced cognitive load with only 5 suggestions per view
	•	Child mode → large buttons, visual cards, simplified navigation

⸻

5. User Flow

We created a full flow showing both adult and child journeys using Mermaid:

It starts with profile selection → adult or child path → discovery and playback → profile switching at any time.

⸻

6. Prototype (Figma)

We designed a clean, modern interface in Figma:
	•	Adult view (neutral tones, focus on personalization)
	•	Child view (bright colors, large controls, categories like “Songs”, “Nursery Rhymes”, “Discovery”)
	•	Clear profile switcher
	•	“Search for Me” and “Mood bubbles” as key interactive elements

⸻

✅ Validation — Usability Study

To validate our solution, we conducted 3 user tests (remote, desktop).
No videos or images were collected — we relied on live observation and note-taking.

Method
	•	3 participants with different Spotify habits
	•	Tasks:
	1.	Choose profile & start a discovery session
	2.	Use “Search for Me”
	3.	Use a “Mood bubble” (e.g., Evening)
	4.	Switch to child profile and play a song
	5.	Retrieve the suggested song later

Metrics: success rate, completion time, SEQ score (1–7), qualitative comments.

⸻

👩‍💻 User 1 – 

Context: Uses Spotify daily with her family.
	•	Found profile selection intuitive: “Oh nice, I can choose who’s listening!”
	•	Slight delay finding the “Search for Me” button.
	•	Loved the child mode colors and big buttons.
	•	Minor confusion when switching back to adult profile.

Success rate	4.5/5 tasks	Median SEQ: 6	Avg time: 68s
Feedback: Smooth experience; improve visibility of “Search for Me” and “Switch profile”.			


⸻

👨‍🔧 User 2 –

Context: Listens mainly to podcasts, not very tech-savvy.
	•	Found profile login simple and clear.
	•	Didn’t understand mood bubbles at first.
	•	Ignored the “Search for Me” button (“Thought it was decoration”).
	•	Didn’t test the child profile.

Success rate	3/5 tasks	Median SEQ: 4.5	Avg time: 92s
Feedback: Clear structure but some labels need clarification (“Search for Me”, “Mood”).			


⸻

👩‍🎓 User 3 – 

Context: Advanced user, heavy playlist creator.
	•	Instantly understood “Search for Me” and used it multiple times.
	•	Loved the 5-song limit: “Now I actually read the list.”
	•	Found the kids’ interface “adorable” but noted low contrast between profiles.

Success rate	5/5 tasks	Median SEQ: 7	Avg time: 50s
Feedback: Very positive. Prototype feels smooth, modern, and playful.			


⸻

📊 Overall results

Metric	Average (3 users)
Overall success rate	80 %
Median task time	≈ 65 s
Median SEQ	6 / 7
Key quotes	“Clear”, “Less crowded”, “Make ‘Search for Me’ more visible”

Insights
	1.	✅ Adult/Kid separation was clear and emotionally engaging.
	2.	⚠️ “Search for Me” button should be more prominent.
	3.	✅ Reducing recommendations improved focus.
	4.	⚠️ “Change profile” needs a clearer label.
	5.	⚠️ Mood bubbles are appealing but need a short tooltip.

⸻

🚀 Conclusion & Next Steps

Outcome

The prototype successfully improved discoverability and clarity.
Participants reported feeling less overwhelmed and more in control of their listening experience.

Key learnings
	•	Personalization isn’t only about algorithms — it’s about reducing effort.
	•	Visual hierarchy and naming strongly affect comprehension.
	•	Even small UX changes can humanize a digital experience.

Next iterations
	1.	Add tooltips and clearer labels for “Search for Me” and “Mood”.
	2.	Increase contrast in profile selection screen.
	3.	Test with a larger sample (5–10 users) after adjustments.
	4.	Prepare for a second iteration focused on onboarding clarity.

⸻

✨ Final thoughts

This case study taught us how designers balance empathy, clarity, and iteration.
Our team discovered that improving UX isn’t about adding more features — it’s about helping users feel understood.


