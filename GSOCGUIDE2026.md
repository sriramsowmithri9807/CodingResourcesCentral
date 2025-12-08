# GSoC 2026: Comprehensive 3-Month Roadmap & Guide

## Introduction

This document provides a detailed, step-by-step roadmap for preparing for Google Summer of Code (GSoC) 2026. It is designed for students and developers who want to secure a slot in a top open-source organization. The timeline assumes you are starting in **January 2026** with the goal of applying when applications open in **March/April 2026**.

**Goal:** Transform from a beginner to a credible contributor with a winning proposal in 12 weeks.

-----

## Part 1: The 3-Month Roadmap

### Month 1: Exploration and Initial Contact (January)

**Focus:** Selecting an organization and setting up your environment.

  * **Week 1: Research and Shortlisting**

      * Visit the GSoC Archive ([summerofcode.withgoogle.com/archive](https://summerofcode.withgoogle.com/archive)) and look at organizations from 2024 and 2025.
      * Filter by your preferred programming language (e.g., Python, C++, Java, JavaScript).
      * Select 2-3 organizations that interest you. Do not pick more than 3; focus is key.
      * **Action Item:** Create a spreadsheet comparing your top 3 choices based on: Activity level (check their GitHub commit frequency), Technologies used, and Availability of "Good First Issues."

  * **Week 2: Environment Setup and Documentation**

      * Choose your primary organization.
      * Join their communication channels (Slack, Discord, IRC, Gitter, or Mailing Lists).
      * **Crucial Step:** Read their "Contribution Guidelines" (CONTRIBUTING.md) and "Developer Guide" thoroughly.
      * **Action Item:** Fork the repository, clone it locally, and successfully build/compile the project. If you encounter errors, try to resolve them yourself first; if you fail, ask in the chat (this is a good first interaction).

  * **Week 3: Codebase Familiarization**

      * Do not dive into complex code yet. Look at the directory structure.
      * Run the test suite to ensure everything passes locally.
      * Locate the issue tracker (usually GitHub Issues or Jira). Filter for labels like `good first issue`, `beginner`, or `junior job`.
      * **Action Item:** Comment on a simple issue asking if it is still open and if you can work on it.

  * **Week 4: The First Contribution**

      * Work on the simple issue you claimed. This might be a documentation fix, variable rename, or small bug fix.
      * Submit your Pull Request (PR).
      * **Action Item:** Ensure your PR follows the project's coding standards. Be patient with feedback.

### Month 2: Deep Contribution and Networking (February)

**Focus:** Becoming a familiar face in the community.

  * **Week 5: Consistency**

      * Once your first PR is merged, pick a slightly harder issue.
      * Start reviewing other people's PRs. You do not need to be an expert; just check for typos or run their code to see if it works.
      * **Action Item:** Aim for 1 merged PR per week.

  * **Week 6: Identifying a Project**

      * Organizations usually publish an "Ideas List" for GSoC. If the 2026 list is not out, look at the 2025 list.
      * Pick 1-2 project ideas that align with your skills.
      * **Action Item:** Publicly introduce yourself in the specific channel for that project (e.g., \#gsoc-project-name) and state your interest in that specific idea.

  * **Week 7: Engaging Mentors**

      * Engage with the potential mentors for your chosen project.
      * Ask technical questions related to the implementation of the idea. Show that you have done your research.
      * **Action Item:** Share a "mini-plan" or a rough diagram of how you plan to solve the project in the chat and ask for feedback.

  * **Week 8: The Pre-Proposal Draft**

      * Start drafting your proposal offline.
      * Continue solving bugs, specifically ones related to the project you want to apply for.
      * **Action Item:** Create a Google Doc draft of your proposal.

### Month 3: Proposal Writing and Final Polish (March)

**Focus:** Writing a winning proposal and finalizing your application.

  * **Week 9: Writing the Proposal**

      * Follow the template provided in Section 4 of this document.
      * Be realistic with your timeline.
      * **Action Item:** Complete the first full draft of your proposal.

  * **Week 10: Feedback Loop**

      * Share your draft link (Comment access only) with the mentors.
      * Ask for a review politely: "I have drafted a proposal for [Project X]. Could you please provide some feedback when you have time?"
      * **Action Item:** Incorporate every single piece of feedback given.

  * **Week 11: Application Submission**

      * Proofread your proposal multiple times.
      * Submit the proposal through the GSoC dashboard.
      * **Action Item:** Do not wait for the deadline. Submit at least 3 days early to avoid server traffic issues.

  * **Week 12: Post-Submission Activity**

      * Do not disappear. Continue contributing code.
      * This period is often used by mentors to decide between candidates with similar proposals. The one who is still coding usually wins.

-----

## Part 2: How to Select Organizations

Choosing the right organization is 50% of the success.

1.  **Tech Stack Match:** Choose an org that uses languages you are already comfortable with. GSoC is not the time to learn a new language from scratch; it is the time to learn a new codebase.
2.  **Recurring Participation:** Look for organizations that have participated in GSoC for at least 3-5 years. They have established processes and experienced mentors.
3.  **Responsiveness:** Check their public chat or mailing list. If a student asks a question and gets no reply for 3 days, avoid that organization. Good orgs reply within 24 hours.
4.  **Commit Frequency:** Check their GitHub "Insights" -\> "Commit Activity." A flat-lining project is a bad choice. You want active development.

-----

## Part 3: How to Approach Mentors

Mentors are volunteers with full-time jobs. Respect their time.

**The Golden Rules:**

1.  **Public Communication:** Never Direct Message (DM) a mentor unless explicitly asked. Always post in the public channel. This shows the community you are active.
2.  **Don't Ask to Ask:**
      * *Bad:* "Can I ask a question?" or "Is anyone here?"
      * *Good:* "I am trying to build the project on Windows 11 but getting Error X at step Y. I have tried Solution Z but it failed. Can anyone help?"
3.  **Do Homework First:** Before asking, Google the error, search the project's issues, and read the documentation. Mention what you have already tried.

**Email/Message Template for Introduction:**

```text
Subject: Interest in GSoC 2026 - [Project Name] - [Your Name]

Hi [Organization Name] Community,

My name is [Name], and I am a [Year] student at [University]. I have been using [Software Name] for a while and would love to contribute to it for GSoC 2026.

I am particularly interested in the [Project Idea Name] from the ideas list. I have already set up the development environment and successfully merged a PR regarding [Topic of your PR].

I am currently reading the code related to [Module Name] to understand how to implement [Feature]. I would appreciate any pointers on where to look for [Specific Technical Detail].

Thank you,
[Your Name]
```

-----

## Part 4: Project Proposal Template

Your proposal is a formal document. Use this structure if the organization does not provide a specific template.

### 1\. Title Page

  * **Project Name:** [Name of the Project]
  * **Name:** [Your Name]
  * **Email:** [Your Email]
  * **GitHub/GitLab Profile:** [Link]
  * **Mentor:** [Mentor Name(s)]

### 2\. Abstract

A 100-word summary of what you will do. Assume the reader is technical but not an expert in this specific module.

### 3\. Detailed Description

  * **Current State:** What is missing or broken?
  * **Proposed Solution:** How will you fix it? Use technical terms (API endpoints, database schemas, algorithms).
  * **Implementation Details:** Include diagrams or flowcharts if possible. Explain *how* you will code it, not just *what* you will code.

### 4\. Deliverables

A bulleted list of tangible results.

  * Mandatory: The core features that must be finished.
  * Optional: "Stretch goals" if you finish early.

### 5\. Timeline (The Most Important Section)

Break down the 12 weeks into weekly milestones.

  * **Community Bonding (May):** Reading docs, refining design.
  * **Week 1-2:** Setup base structure, create boilerplate code.
  * **Week 3-4:** Implement Core Feature A.
  * **Week 5-6:** Implement Core Feature B + Tests.
  * **Mid-Term Evaluation:** Buffer time for delays.
  * **Week 7-8:** UI/UX integration or Optimization.
  * **Week 9-10:** Documentation and Bug fixes.
  * **Week 11-12:** Final polish, extensive testing, and code merging.

### 6\. Biographical Information

  * Who are you?
  * Why are you the right person? (Highlight relevant coursework or past projects).
  * **Availability:** State clearly that you can commit 30-40 hours per week (or 15-20 for medium projects). Mention any exams or vacations planned.

-----

## Part 5: Top 50 Active Organizations

This list is based on consistent GSoC participation and high student acceptance rates.

### Web Development & CMS

1.  **Drupal** (PHP/Symfony)
2.  **Joomla\!** (PHP/JS)
3.  **Plone Foundation** (Python/React)
4.  **WordPress** (PHP/React)
5.  **Django Software Foundation** (Python)
6.  **Rocket.Chat** (JavaScript/Meteor/Node)
7.  **OpenMRS** (Java/React - Healthcare)
8.  **Zulip** (Python/Django)
9.  **Oppia** (Angular/Python - Education)
10. **Moodle** (PHP - Education)

### Python & Data Science

11. **Python Software Foundation** (Core Python)
12. **NumFOCUS** (Pandas, NumPy, Jupyter, SciPy)
13. **TensorFlow** (Machine Learning)
14. **Scikit-learn** (Machine Learning)
15. **OpenCV** (Computer Vision)
16. **MetaCall** (Polyglot Programming)
17. **SunPy** (Solar Physics)

### C++ & Systems

18. **LLVM Compiler Infrastructure** (Compilers)
19. **Boost C++ Libraries** (Core C++)
20. **Haiku** (Operating System)
21. **KDE Community** (Qt/C++)
22. **The Linux Foundation** (Kernel/Drivers)
23. **Git** (Version Control)
24. **Ceph** (Distributed Storage)
25. **Inkscape** (Vector Graphics)

### Javascript / Frontend / Mobile

26. **The Chromium Project** (Browser engine)
27. **VideoLAN (VLC)** (Multimedia)
28. **React Native** (Mobile)
29. **Processing Foundation** (p5.js - Creative Coding)
30. **App Inventor** (MIT - Visual Blocks)
31. **FOSSASIA** (Various Web/Mobile technologies)
32. **Wikimedia Foundation** (Wikipedia - PHP/JS)

### DevOps, Cloud & Infrastructure

33. **CNCF (Cloud Native Computing Foundation)** (Kubernetes, Prometheus)
34. **Jenkins** (CI/CD - Java)
35. **Docker** (Containers)
36. **PostgreSQL** (Database)
37. **MariaDB** (Database)
38. **Apache Software Foundation** (Big Data/Server - Hadoop, Spark, Kafka)

### Security

39. **The Honeynet Project** (Network Security)
40. **OWASP Foundation** (Web Security)
41. **Metasploit** (Penetration Testing)

### Robotics & Science

42. **ArduPilot** (Drones)
43. **CERN** (Physics Research)
44. **INCF** (Neuroinformatics)
45. **Open Robotics (ROS)** (Robot Operating System)

### Other Reliable Organizations

46. **Mozilla** (Firefox/Rust)
47. **Blender Foundation** (3D Graphics)
48. **FreeBSD** (Operating System)
49. **GNOME** (Linux Desktop)
50. **Sugar Labs** (Education OS)
