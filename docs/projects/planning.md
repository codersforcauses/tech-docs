# Planning a Project

So you've decided on a project and you've nominated yourself to be the tech lead. You might've sat in on the original client meeting, or you might not have. Fact remains you should plan a follow-up meeting **as soon as possible**. The earlier you start, the better and the more planning you do the better.

## First Client Meeting

Continuing on from the [previous page](./clients.md), you now need to think on a deeper level. The [Notion Page](https://www.notion.so/codersforcauses/Project-Requirements-Elicitation-Doc-1c7bddb3a4294e979ef8af1e14ce208f) written by @junhyap already gives a great high level overview, so here are some questions to ask and some words of advice:

- Write **everything out**. Make sure both you and the client are on the same page. In the same respect, repeat back to the client your interpretation of what they said. Ensure no misunderstandings -- you don't have time for that.
- What are your assumptions? What are _their_ assumptions?
- What do they want? What is essential? What is not-so-essential? **Prioritise them**. Use those cringe agile models -- they work :pensive:.
  - <https://publicagile.org/agile-playbook/agile-planning/100-dollar-test/>
  - <https://www.atlassian.com/agile/product-management/requirements>
- Scope. Keep things simple. You have to consider the experience of the volunteers. You will suck at this the first time you're doing it.
- Who are the users of the app?
  - If there are multiple types consider their user journey. e.g. Is there an admin and regular user? Do you need to consider permissions?
  - Will there both mobile and desktop users?
  - Also make user stories if you need to -- they're particularly useful for onboarding volunteers.
- What is the final product? Is it a website? Is it a PWA? PWAs are a good alternative to mobile apps because they're more accessible for developers and we can dodge the $99 fee Apple has to put an app on the App Store.
- What should it look like? Ask if they have particular branding, or a specific style. This is also where you need to consider the users of the app. Are they children or the elderly?
- What's their budget? This affects your deployment options.
- What about after handover? Do they have a tech team to continue maintaining it? Would they be happy to hire some of the volunteers after to continue working on it?

Finally and most importantly, **_BE DECISIVE_**. Clients will often throw around ideas or come to you with a vague notion of what they want. It's your job as a tech lead (and the project manager's) to turn it into something concrete. If they can't decide, decide for them. Give a recommendation, explain your reasoning and have **_CONVICTION_**. If you make the wrong decision, say it and see what you can do to recalibrate.

## Architecting

### ERD

Easiest one to knock out after getting your requirements is making an [ERD](https://www.lucidchart.com/pages/er-diagrams). It gets you thinking about the data flow, and it can readily be turned into a database schema. The simpler you can make it (or negotiate it), the easier time volunteers will have. Be aware of the nice-to-haves from your requirements doc, but try to keep them out at this stage. Focus on the bare functionality you need to have a functional app -- you can can always refine it later.

### User/API Flows

Consider creating a sequence diagram with mermaid or some other tool if a certain part of the app is complex. An ideal project will be simple enough that the Figma design will cover it, but if you have the time, feel free to do so.

### Tech Stack

Pick a tech stack! I strongly recommend using one that is already in the GitHub repo templates. For more information about choosing your own, see [Picking a New Stack](../stack/new-stack.md).

### Repo Setup

This should be straightforward unless you're setting one up from scratch, as everything is done for you. Just make sure to create a GitHub team under the `codersforcauses` org and invite all the volunteers. Then configure the repo to give write access to them. You also want to make sure merging to main without approval and a passing CI is blocked and pushing directly to main is blocked.

Start adding some GitHub issues to the repo. Look at past projects for inspiration. Usually it goes design, navbar, DB schema, homepage, authentication, sign-up, etc...

### Figma

If you've done everything so far you're already doing quite well. You don't have to get fully into the design, but make sure you have an idea of the colour palette you'll be using and a rough vibe of what it'll look like. Most of this work can be left to the volunteers, but if you're pressed for time (like during Winter projects) you can do it yourselves. A pre-done Figma design is probably the most helpful for getting volunteers to start coding.
