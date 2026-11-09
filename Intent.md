# Intent.md — Optional PRD Draft (Build 1)

**Build 1 due:** Monday, Nov 9, 2026 at noon, New York time  
**Builder:** Adwika Narain

---

## 1. Who is it for?

- **Target user:** An emerging or self-publishing author preparing a manuscript for publishing. I got the idea from an author I worked with during my book marketing internship, where I helped support the launch of her novel and noticed that she found editing extremely cumbersome and even after multiple iterations, as an early reader I still found many issues.

- **How I will reach them to test it:** I plan to reconnect with the author from my internship to demonstrate the prototype and gather feedback on whether the tool identifies useful issues and fits into her existing editing process. User testing has not yet been conducted.

## 2. What job does it do?

- **Current painful workflow (before):** Authors often go through multiple rounds of proofreading and editing to identify grammatical errors, spelling mistakes, and inconsistencies in their manuscripts. During my summer internship, I encountered a manuscript that still contained numerous errors despite having gone through several rounds of editing. This process can be time-consuming and costly, particularly for independent authors who lack access to the editorial resources of large publishing houses.

- **New workflow with this product (after):** An author uploads or pastes a manuscript excerpt into Margins, which reviews the text and flags potential grammatical, spelling, continuity, and plot inconsistencies. The author can review each suggestion and decide whether to make changes, retaining complete creative control. The initial prototype focuses only on identifying a limited set of continuity contradictions in short excerpts.

- **Why this is useful:** Margins aims to reduce the time authors and editors spend identifying mechanical errors and inconsistencies, allowing them to focus more on storytelling, creative development, and preparing the book for publication. The longer-term goal is to make high-quality editorial support more accessible to emerging authors. Time savings and willingness to pay still need to be validated through user testing.

## 3. What is in and out of scope?

- **One core workflow:** The author enters a short manuscript excerpt → selects Review Manuscript → receives a clearly explained potential continuity issue with supporting evidence → decides whether to revise the text.

- [ ] **Not building:** Automatic rewriting of manuscript passages or changes to the author's creative voice.
- [ ] **Not building:** Full-length manuscript analysis, including cross-chapter character tracking and complex plot consistency checks, during the initial six-week build.
- [ ] **Not building:** Integrations with publishing platforms, word processors, or professional editorial workflows.

## 4. Rough Local Prototype

- **Local run command / branch / screenshot:** The Build 1 prototype is a browser-based HTML application that runs locally by opening `prototype/index.html`. The code is saved in the `main` branch of the GitHub repository. A three-step screenshot walkthrough is included on the Product Page.

- **What worked vs. what surprised me:** I successfully built a functional prototype that allows users to enter manuscript text, load a sample excerpt, and review a predefined continuity contradiction. The prototype highlights the inconsistency and provides supporting evidence without automatically changing the author's writing.

  One important learning was that detecting continuity issues is more complicated than identifying grammatical mistakes because it requires understanding context and relationships between statements. The current rule-based prototype can demonstrate the intended workflow, but it cannot reliably analyze arbitrary manuscripts. Future iterations will need more advanced AI capabilities to make the tool useful beyond predefined examples.
