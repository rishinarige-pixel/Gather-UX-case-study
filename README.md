# Gather: Turning "we should hang out" into an actual plan

![image alt](https://github.com/rishinarige-pixel/Gather-UX-case-study/blob/bd343ed5dbb2b53e3cf6370594aedd6f30abffec/iPhone%2018%20Pro.png)

A mobile app case study. UX/UI Design. [Figma Project](https://www.figma.com/design/d6KH1O9Aw03wX2ZtBrFGSH/Gather)

## The Problem

I kept noticing hangout ideas quietly die in my own friend group chats, which is what led me to dig into the research below.

Making spontaneous plans with friends should be effortless, but it isn't. Most hangout ideas die in group chats because no one wants to carry the full burden of organizing. People wait for others to commit first, messages get buried, and momentum fades. There's no lightweight middle ground between sending a text and creating a full calendar event.

### Design opportunity

Plans fail not because people don't want to hang out, but because the tools demand too much commitment too early. If we reduce the friction of sharing an idea and make it easy to signal interest without fully committing, more plans will actually happen.

### How might we

1. How might we help friend groups turn casual ideas into real hangouts, without the pressure of full planning or the chaos of group chats?
2. How might we let people share availability without it feeling like a commitment?
3. How might we create a natural progression from a loose idea to a confirmed plan that feels social, not administrative?

## Who It's For

Gather is built for friend groups in their mid-20s who want to hang out spontaneously but keep losing the thread in group chats. Three types of people showed up consistently in my research: initiators who post ideas but get tired of always organizing, busy joiners who want a simple yes or no without reading forty messages, and over-planners who need to know who's coming before they'll commit. Full persona details, including quotes and behaviors, are below.

## Research Synthesis

![image](https://github.com/rishinarige-pixel/Gather-UX-case-study/blob/28004e3a6e78e837bac4ef63855de8b22f4c0f22/research-insights.png)

### Competitive audit: what's missing

1. **WhatsApp / iMessage**: Plans get buried in conversation history. No structure, no visibility into who's actually free.
2. **Google Calendar**: Built for confirmed events, not loose ideas. Too formal for a same day chai run.
3. **Partiful**: Great for parties, but requires a committed host and a full event setup. Not spontaneous.
4. **Lunch Club / Friender**: Discovery focused, not friend group focused. Too much friction for existing social circles.

### The gap

No app exists that lets you post a loose idea to your friend group, collect soft interest signals, and let a plan naturally crystallize, without requiring a dedicated organizer.

## User Personas

Three distinct users, one shared pain point.

![image alt](https://github.com/rishinarige-pixel/Gather-UX-case-study/blob/47e049bea1214baa8ed6d5584d7ab7e9f93f9957/user-personas-v2.png)

## User Journey Map

Sara's journey from idea to hangout: a simple progression that keeps commitment low until momentum forms.

| Stage | Action | Thought | Emotion | Pain point | Opportunity |
|---|---|---|---|---|---|
| 1. Impulse | Sara has a free evening and feels like going out | Who's free tonight? | Happy | No easy way to broadcast availability | Quick "I'm free tonight" status post |
| 2. Posting | Opens Gather, taps + to post a plan idea | Let me keep it casual | Content | Other apps require too many fields | Two tap post: text plus optional time |
| 3. Waiting | Checks if anyone reacted to her post | Did anyone see it? | Anxious | No visibility into who's seen it | Show "seen by 4" without pressure |
| 4. Interest | Arjun and Nisha tap "I'm in" or "Maybe" | Okay, this might actually happen | Relieved | No middle ground between yes and no | "Maybe" plus a suggest another time action |
| 5. Confirming | Plan reaches threshold, Gather prompts to confirm details | Now I'll add the location | Excited | Detail first apps kill momentum early | Details unlock only after interest forms |
| 6. Confirmed | Plan moves to confirmed state with location and chat | We're actually doing this! | Delighted | No clear transition moment in other apps | Celebrate confirmation with a clear state change |

## Information Architecture

Mental model: people start with a plan idea, gather interest, confirm, then hang out.

**Home**
Feed of plan cards (states: idea, getting interest, confirmed, archived) with actions to react, comment, or share. Filters for all, close friends, nearby, and tonight/weekend. Quick actions for posting a plan and search.

**Calendar**
Agenda, day view, and week view, linking through to plan details.

**Plans**
My plans (posted, joined, saved), past plans, and drafts for ideas started but not published.

**Profile**
Friend groups, availability, privacy, and notifications.

**Accessible globally:** plan details (from a card or the calendar) and the create plan screen.

Plan card lifecycle: idea posted, getting interest, threshold reached, confirmed, archived.

![image alt](https://github.com/rishinarige-pixel/Gather-UX-case-study/blob/a037c22abe1310bbdfb2ca4d1a1666950720711a/Information%20Architecture.png)

## User Flows

Three core flows cover the full product experience.

**Flow 1, Posting a plan idea (Sara).** She opens Gather and taps the plus button, types a quick idea like "anyone up for chai tonight?" into a single text field with no required fields yet, optionally adds a time or visibility chip, then posts. The card appears on the board with her avatar, and a soft push notification goes to the selected friend group.

![image alt](https://github.com/rishinarige-pixel/Gather-UX-case-study/blob/34c3c6ac234138edd2bd3dd20fb55f4914a5f158/User%20Flow%201.png)

**Flow 2, Reacting to a plan (Arjun).** He gets a notification and opens the board to see Sara's card, taps it to expand and see who else has reacted, then reacts with a one tap "I'm in," "Maybe," or "Suggest a time." Sara gets notified of his response, and if enough interest builds, the card upgrades to a "getting hot" state, prompting Sara to confirm details.

![image alt](https://github.com/rishinarige-pixel/Gather-UX-case-study/blob/47c89666bab6fbb78a2691253c199f9bc8cdd21d/User%20Flow%202.png)

**Flow 3, Confirming a plan (Sara).** A threshold notification tells her three friends are in, with a "Make it official" call to action. She confirms the time and adds a location, with fields pre-filled from what was already shared. The plan moves to a confirmed state, a group chat thread opens automatically, and all participants are notified. The plan then lives in "My Plans" until it's archived after the date passes.

## Feature Prioritization (MoSCoW)

**Must have:** quick plan post (text plus optional time), react options (in, maybe, suggest time), the plan card feed, the plan state lifecycle, friend group visibility controls, and push notifications.

**Should have:** group chat on confirmed plans, an availability status ("free tonight"), a My Plans calendar view, an expiry nudge for dead plans, and a "seen by" counter without read receipts.

**Could have:** photo or vibe attachments on posts, location suggestions via Google Places, plan templates like "coffee run" or "movie night," and the option to add confirmed plans to your phone calendar.

**Won't have in v1:** a public discovery feed for strangers, ticketing or RSVP payments, an AI scheduling assistant, and a map or nearby view.

## Design Principles

1. **Signal before commitment.** Never ask for full details upfront. Let interest form first, then unlock structure. A plan starts as a sentence and becomes an event only when it earns it.
2. **Speed over completeness.** The fastest path to a posted plan should be two taps. Every extra field is a reason not to post; friction kills spontaneity.
3. **Visibility without pressure.** Show social proof gently. "3 people are interested" is motivating. Read receipts and hard RSVPs are anxiety inducing. Design for curiosity, not obligation.
4. **No single organizer.** The burden of organizing shouldn't fall on one person. Gather distributes responsibility so anyone can post, react, or suggest a change. Plans belong to the group.
5. **Private by default.** Plans are visible only to selected friends unless the poster explicitly opens them up. Trust is the foundation of spontaneity; if it feels public, people won't post casually.

## Key Screens

| Screen | What it does |
|---|---|
| [Welcome](https://www.figma.com/design/d6KH1O9Aw03wX2ZtBrFGSH/Gather?node-id=251-22244) | First impression, sets the tone for a casual, low effort app |
| [Onboarding](https://www.figma.com/design/d6KH1O9Aw03wX2ZtBrFGSH/Gather?node-id=251-22258) | Fast phone based sign up, minimal friction |
| [Home](https://www.figma.com/design/d6KH1O9Aw03wX2ZtBrFGSH/Gather?node-id=251-21329) | Feed of live plan ideas from friends, with quick react buttons |
| [Post a Plan](https://www.figma.com/design/d6KH1O9Aw03wX2ZtBrFGSH/Gather?node-id=251-21428) | Compose sheet for floating a new idea |
| [Plan Detail](https://www.figma.com/design/d6KH1O9Aw03wX2ZtBrFGSH/Gather?node-id=251-21584) | Full view of an idea: who's in, who's maybe, suggested times |
| [Make it Official](https://www.figma.com/design/d6KH1O9Aw03wX2ZtBrFGSH/Gather?node-id=251-22003) | Confirmation flow once enough interest has built up |
| [My Plans](https://www.figma.com/design/d6KH1O9Aw03wX2ZtBrFGSH/Gather?node-id=251-22072) | Posted, joined, and saved plans at a glance |
| [Calendar](https://www.figma.com/design/d6KH1O9Aw03wX2ZtBrFGSH/Gather?node-id=251-21791) | Confirmed plans laid out by date |
| [Chats](https://www.figma.com/design/d6KH1O9Aw03wX2ZtBrFGSH/Gather?node-id=251-21674) | Auto created group threads for confirmed plans |
| [Profile](https://www.figma.com/design/d6KH1O9Aw03wX2ZtBrFGSH/Gather?node-id=251-22140) | Hosting history, social stats, availability toggle |

## Reflection

This is where a case study really shines for recruiters. A few prompts to answer in your own words:

1. What was the hardest design decision in this project, and how did you resolve it?
2. If you had more time, what would you explore further?
3. Did anything change significantly between your first draft and the final version, based on the research above?
