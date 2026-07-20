<p align="center">
  <a href="https://github.com/EnAccess/oseas26-mpm-whatsapp-plugin">
    <img
      src="https://drive.google.com/uc?id=1gtL_p7l3HbOcCzc09A7KW5d7B5qn-BDs"
      alt="WhatsApp Channel Plugin for MicroPowerManager (MPM)"
      width="640"
    >
  </a>
</p>
<p align="center">
    October 26-27 | Open Source in Energy Access Symposium Hackathon | Kigali, Rwanda
</p>

---

# WhatsApp Channel Plugin for MicroPowerManager (MPM)

Build a [MicroPowerManager (MPM)](https://micropowermanager.io/) plugin that
delivers MPM's existing notifications over the WhatsApp Business API.

This challenge is based on
[MPM issue #1340](https://github.com/EnAccess/micropowermanager/issues/1340).

## Abstract and goal

MicroPowerManager (MPM) is an open-source CRM platform for managing off-grid
energy deployments. It already sends transactional messages — payment receipts,
low-balance warnings, token deliveries — over SMS and email. But across most of
the markets MPM serves (sub-Saharan Africa, South and Southeast Asia), WhatsApp
is the dominant messaging channel. It's how customers already talk to family, to
merchants, and to support. SMS is the fallback, not the front door.

For operators, that gap costs money in real ways: SMS unit costs are high relative
to data-channel alternatives, delivery rates on some networks are poor and
silently so, and customers who would read a WhatsApp message from a known business
ignore an SMS from an unfamiliar number.

This challenge aims to close that gap by building a MicroPowerManager plugin that
delivers MPM's existing notifications over the WhatsApp Business API, and lets
operators configure it the way they configure any other channel today. The plugin
should:

- Deliver MPM's existing notifications (e.g. payment receipts, low-balance
  warnings) over WhatsApp.
- Let operators enable and configure the channel from MPM's plugin admin with
  their own WhatsApp Business credentials — no code changes required.
- Respect WhatsApp's business rules: real opt-in, approved message templates, and
  the 24-hour session window.
- Make delivery failures visible, with a clear fallback posture (fall back to SMS,
  queue for retry, or log).

The result gives operators a lower-cost, higher-engagement channel to reach
customers where they already are, using open-source tooling end to end.

## Expected outcomes

Create a Feature Request and an accompanying PR on the
[MPM repository](https://github.com/EnAccess/micropowermanager/) to:

- Integrate a WhatsApp channel plugin on MPM, following the shape of MPM's
  existing notification channels.
- Allow an operator to enable and configure the plugin from MPM's plugin admin
  with their own WhatsApp Business credentials.
- Deliver at least two existing MPM notifications (for example, payment receipt
  and low-balance warning) to a real WhatsApp number via the plugin.
- Log and handle delivery failures visibly, according to the fallback design the
  team chooses.

## Required knowledge

### Stack

- PHP/Laravel backend.
- Vue.js 2 frontend.
- WhatsApp Business Platform (Meta Cloud API or an aggregator such as Twilio,
  360dialog, Infobip).

### Programming languages

- PHP (Laravel)
- JavaScript

### Helpful experiences

- Backend/API integration with PHP/Laravel.
- Knowledge of frontend development.
- Experience integrating messaging APIs (WhatsApp Business API, Twilio, or
  similar) and handling webhooks.

## Person of contact supporting this challenge

- Obinna Ikeh

## Getting started

- Join the OSEAS Discord server: <https://community.oseas.org/>
- Introduce yourself in the `#introductions` channel and join the relevant
  channels for this challenge"
  - `#micropowermanager`
- Read the documentation:
  - <https://micropowermanager.io/get-started.html>
  - <https://github.com/EnAccess/micropowermanager/>
  - <https://github.com/EnAccess/micropowermanager/issues/1340>
  - <http://micropowermanager.io/development/plugins.html>
  - <https://developers.facebook.com/docs/whatsapp>
