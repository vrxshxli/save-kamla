<p align="center">
  <img src="assets/banner.png" alt="Can you save Kamla? A 2-minute flood-night game about Pukaar, our AI agent team for disaster response" width="100%">
</p>

<p align="center">
  <a href="https://vrxshxli.github.io/save-kamla/"><img src="https://img.shields.io/badge/%E2%96%B6%20Play%20now-2%20minutes-E0A21C?style=for-the-badge" alt="Play now, 2 minutes"></a>
  <img src="https://img.shields.io/badge/AgentX%20Hackathon-2026-0F7173?style=for-the-badge" alt="AgentX Hackathon 2026">
  <img src="https://img.shields.io/badge/Problem-PS--03%20Disaster%20response-B3284F?style=for-the-badge" alt="PS-03 Multi-agent disaster response coordinator">
</p>

<h3 align="center">You are the duty officer on a flood night. You have three boats.<br>Somewhere in hundreds of messages, a 68-year-old woman is waiting.</h3>

<p align="center">
  <a href="https://vrxshxli.github.io/save-kamla/"><b>▶ Play it in your browser</b></a> · no install, no login · works on a laptop or a phone turned sideways
</p>

<br>

## 🌊 Why this game exists

India can send a flood alert to every phone. The SACHET system has sent over **134 billion alerts in 19+ languages**. But when people reply asking for help, it comes back as chaos: WhatsApp voice notes, posts, forwards and calls, all landing in one control room.

On a real flood night:

| What happens | What it costs |
|---|---|
| 📨 The same family is reported 5 times, in 3 languages | Nobody knows it’s one family |
| ⌨️ Volunteers hand-type each request, about **3 minutes** each | Hundreds arrive every hour |
| 🚤 Boats go to people who were **already rescued** | Someone else keeps waiting |
| 📢 Rumours (“the dam has burst!”) spread faster than facts | Panic, wasted trips |

**Pukaar** (पुकार, “a call for help”) is our idea for fixing this: a team of AI agents that turns every call for help into **one ticket**, gets it to the **right rescuer**, and **closes it** when the family is safe, with a human approving every boat.

This game lets you **feel** that difference in two minutes.

<br>

## 🎮 How it plays

<p align="center">
  <img src="assets/story.png" alt="Animated story intro: a flooded house at night sending a call for help to the control room" width="88%">
</p>

The game opens with a short animated story: it’s 9:30 PM, Ward 12 is flooding, and Kamla, 68, is on the ground floor with her feverish grandson. Then you play the same night twice.

### Round 1 · The way it works today

<p align="center">
  <img src="assets/round-1.png" alt="Round 1: a live flood map with boats sailing, next to a feed of raw messages" width="100%">
</p>

- Messages pour in: voice notes in Hindi, posts in English, SMS in Hinglish, emotional reposts, rumours and questions.
- **You** read them, pick one, and press **Send a boat here**.
- Your boat sails across the live map, and you see what it finds: *“Already rescued at 8:12 PM”*, *“Lane 6 is flooded, turning back”*, *“Kamla found, after a search”*.
- Floodwater keeps rising while you decide.

### Round 2 · The same night, with Pukaar

<p align="center">
  <img src="assets/round-2-map.png" alt="Round 2: the map shows ranked ticket pins, a flooded lane already avoided, and an explanation of what the agent just did" width="88%">
</p>

- The **same messages** arrive, but now six AI agents read them first.
- Every message gets a label showing which agent handled it, and a **“What just happened”** bar explains each agent in plain words the first time it acts.
- Urgent families become **pins on the map**, ranked with reasons. Kamla’s three messages merge into one ticket (`×3`).
- When a boat is proposed, **you check the reasons and tap Approve**. That’s your whole job.

<p align="center">
  <img src="assets/saathi.png" alt="Saathi, the safety companion, guiding Kamla through a gas leak in Hindi while she waits for the boat" width="70%">
</p>

While Kamla waits, **Saathi**, the safety companion, walks her through a gas leak in Hindi, using only an approved safety playbook, and flags the risk to the boat crew.

### The result

<p align="center">
  <img src="assets/results.png" alt="Side-by-side results: boats wasted and families reached in round 1 versus round 2" width="100%">
</p>

The comparison is built from **your own choices** in each round.

<br>

## 🤖 Meet the agents

| | Agent | What it does in the game |
|:-:|---|---|
| 👂 | **Listen** | Understands voice notes and messages in Hindi, Marathi, Hinglish and English, and pulls out who needs help, where and how urgently |
| 🔀 | **Triage** | Merges repeat reports into one ticket, ranks tickets with reasons, and sends rumours to be checked |
| 🗺️ | **Watch** | Remembers road and power reports, so routes avoid flooded Lane 6 automatically |
| 🚤 | **Dispatch** | Proposes the right boat for each family, and never sends one without your approval |
| 🔁 | **Loop** | Tells everyone reposting about a rescued family that they’re already safe, and answers general questions |
| 🛟 | **Saathi** | Stays with the family while they wait, with safety steps from approved playbooks; danger always goes to 112 first |

<br>

## 🧭 How a call for help flows

```mermaid
flowchart LR
    A["📱 Message<br/>voice · post · SMS"] --> B["👂 Listen<br/>understands it"]
    B --> C{"🔀 Triage"}
    C -->|"same family"| D["Merge into<br/>existing ticket"]
    C -->|"new call for help"| E["New ticket<br/>ranked with reasons"]
    C -->|"already rescued"| F["🔁 Loop<br/>auto-reply"]
    C -->|"rumour"| G["Verify lane"]
    D --> H["🚤 Dispatch<br/>proposes a boat"]
    E --> H
    H --> I(["✋ Officer<br/>approves"])
    I --> J["Boat sails<br/>route avoids danger"]
    J --> K["✅ Family safe<br/>ticket closed"]
    E -.-> L["🛟 Saathi<br/>keeps them safe<br/>while they wait"]
    L -.-> K
```

<br>

## ⚖️ Same night, two endings

| | Round 1 · Today | Round 2 · With Pukaar |
|---|---|---|
| **Who reads every message** | You | The agents |
| **Repeat reports** | Look like new emergencies | Merged into one ticket |
| **Already-rescued reposts** | Can waste a boat | Answered automatically |
| **Rumours** | Can waste a boat | Sent to be checked |
| **Flooded roads** | Found by boats the hard way | Remembered and avoided |
| **Kamla while she waits** | Alone | Guided by Saathi |
| **Your job** | Everything | Approve three boats |

> **Agents do the paperwork. Humans send the boats.** Nothing irreversible happens without a person approving it.

<br>

## 🛠️ Under the hood

- **One self-contained `index.html`**: vanilla JavaScript, CSS and animated SVG. No framework, no backend, no tracking.
- **Live map** drawn in SVG, with boats animated along road routes and rising water.
- **Accessible**: keyboard friendly, respects *reduced motion*, and follows your light or dark mode.

**Run it locally:** download `index.html` and open it in any browser.

<br>

## 📌 Please note

This is a **scripted simulation of the Pukaar concept**, made for the AgentX Hackathon 2026 idea round so anyone can understand the problem and the idea in about two minutes. The messages, families and outcomes are **illustrative**, based on documented flood-night patterns, and all data is mock. The real multi-agent system, with live tools and human approval gates, will be built during the 24-hour hackathon round.

<br>

<details>
<summary><b>📚 Sources for the facts above</b></summary>
<br>

- NDMA / C-DOT on the SACHET alert system, 2026
- Khaleej Times on Kerala flood volunteers, 2018 (manual entry of rescue requests)
- Office of the Kerala Chief Minister, via The Statesman, 2018 (requests for people already rescued)
- The News Minute on lessons from the Kerala floods, 2018

</details>

<br>

<p align="center">
  <b>No call for help should be heard five times and answered never.</b><br><br>
  <a href="https://vrxshxli.github.io/save-kamla/"><img src="https://img.shields.io/badge/%E2%96%B6%20Can%20you%20save%20Kamla%3F-Play%20now-E0A21C?style=for-the-badge" alt="Play now"></a>
</p>
