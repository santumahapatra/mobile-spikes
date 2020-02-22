# Today's Backend Infrastructure

## Introduction

This document is intended to act as a starting place and template for describing the state of the world _as it is_ (around February 2020). We will create other documentation elsewhere to describe the world _as we hope it to be one day_. The term "backend" is intentionally vague, since Pariyatti's infrastructure involves bare-metal physical machines, virtual servers, SaaS providers, and more. This document need not be beautiful, but hopefully it will be thorough. :) If adding images to this document helps, save them in the same `docs/backend` directory and reference them from this document.

The structure of this template will break down all the major components of Pariyatti's infrastructure by `nouns` --- it's very likely that this isn't the best way to capture this information, so feel free to re-organize the document (or even pick a different document format entirely, if it's easier) where it makes sense.

Open questions not necessarily pertaining to infrastructure can be found in the `QUESTIONS.md` document at the root of this repository.


## People

`People` are points-of-contact (a human being) for the other `nouns` in this list. Pieces of backend infrastructure should be connected to a real human being(s). Wherever contact information is missing, assume Steve H is the point-of-contact.

### Internal

- Steven D: writing this template, volunteer helping with Pariyatti's backend and mobile app, new to Pariyatti; knows little
- Steve H: 8 years as Pariyatti staff and probably the person to fill out most of this template.
- Ankur N: AT and Pariyatti staff; will help Steve H capture information in this doc
- ???
- ???

### External

Example: Support staff from Dreamhost/3dcart/etc Pariyatti engages with individually

- ???
- ???


## Not People

`Not People` are points-of-contact Pariyatti regularly uses that obfuscate the humans behind it. For example, a `support@company.com` email address.

- ???
- ???


## Pariyatti Services

`Pariyatti Services` are the high-level services Pariyatti owns and provides to its users, irrespective of where or how they are hosted.

1. DotNetNuke (DNN) --- pariyatti.org
2. 3dcart --- store.pariyatti.org
3. Moodle --- learning.pariyatti.org
4. Dreamhost --- generic web/file server
5. ???


## Hardware

`Hardware` could be any physical computer or device Pariyatti makes regular use of. "Physical" is important because it captures specific risks: the computer can break down in a way that requires a real-world replacement; the computer can be stolen causing a loss of data.

### Servers

- ???
- ???

### Official Desktops/Laptops

"Official" here means that if the computer was lost/destroyed/stolen something saved on it (passwords, keys, data, etc.) would be impossible to recover. Desktops owned by Pariyatti but with no special significance need not be captured here.

- ???

### Devices (Phones, Yubikeys, etc.)

- ???


## Virtual Servers

Dreamhost servers probably come here. Mentioning which type of Dreamhost service would be helpful (VPS, shared, cloud, etc.)

- static IP? / hostname? / purpose?
- ??? / ??? / ???


## Software-as-a-Service (SaaS)

`SaaS` includes any servers or services over which Pariyatti has limited control. So we don't get too fancy, we'll lump all other `X-as-a-Service` categories under SaaS for now. Examples include `managed.com` for DNN, as well as the DNN instance itself, 3dcart, managed CDNs, etc. If you aren't sure whether or not something is SaaS, list it here and we'll discuss! :)

- managed.com
- DotNetNuke
- 3dcart
- moodle
- ???


## Network Services

`Network Services` can be used to capture anything which isn't user-facing. These may include network layers like DNS but might also include things like web servers which can't be accessed by Pariyatti users directly.

- Domain Registrar?
- DNS / nameservers?
- SSL certificate service?
- Load balancers?
- Servers without public URLs or interfaces?


## Security Tools

`Security Tools` include password managers, SSL certificate management (if done locally), 2-Factor-Auth tools, etc.

- ???
- ???


## Logins

`Logins` captures a broad range of the previous categories. Obviously, do not write down usernames in this file unless those usernames are inherently public already (ex. GitHub). Without specifics, we can identify how many logins we have + the login URL for each of the different services/servers used.

If anyone feels uncomfortable with this approach, please leave this section blank and we can enter this data into a private document.

- ex: user1 @ panel.dreamhost.com
- ex: user2 @ panel.dreamhost.com
- ex: user1 @ support.dreamhost.com
- deobald @ github.com/login
- santumahapatra @ github.com/login
- ???
- ???


## Communication Tools

`Communication Tools` is a list of all the existing communication tools in use and their purpose.

- Email: Asynchronous messaging
- WhatsApp: Small asynchronous (and synchronous) messaging
- GoToMeeting: Video calls / screensharing
- Google Hangouts: Video calls / screensharing
- ???
- ???


## Project Management Tools

`Project Management Tools` includes anything used to track work items or tasks and share them between team members.

- Asana
- Google Docs


## New Category One

Feel free to add categories if you think of some information that doesn't fit into the categories above!


## New Category Two