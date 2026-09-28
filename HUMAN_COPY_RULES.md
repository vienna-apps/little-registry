# Little Registry: Human Copy & Product Writing Rules

This file is the writing source of truth for Little Registry.

It adapts the useful principles from Peter Yang's **no-ai-slop** project to this product. The original project is MIT licensed. We are not copying its workflow blindly; these rules are tuned for an Indonesian baby-registry product used by parents and guests.

Source: https://github.com/petergyang/no-ai-slop

## Goal

Little Registry should sound like a thoughtful person wrote it for another person.

The product is warm, practical, calm, and specific. It can be cute without becoming childish. It can be friendly without sounding like marketing copy.

For Indonesian UI, natural mixed Indonesian-English is allowed when that is how the feature is commonly understood: "Parent View", "Guest View", "Most Wanted", "patungan", "gift", "registry". Do not translate a familiar term just to sound formal.

## Core rules

1. Lead with what the user needs to know or do.
2. Prefer concrete language over abstract claims.
3. Use active voice and direct verbs.
4. Keep useful personality. Do not polish every sentence into the same tone.
5. Make the minimum effective edit. Clear copy does not need to sound corporate.
6. Keep one name for one concept. If we call it a registry item, do not rotate between "item", "gift object", "present choice", and "selection" for variety.
7. Do not invent urgency, popularity, safety claims, statistics, reviews, or product benefits.
8. Explain consequences instead of labeling something "important".
9. Short UI copy should be especially plain. Buttons should say what happens.
10. Cute details are accents, not the information architecture.

## Little Registry voice

### Parent-facing

Parents are configuring something personal. Copy should feel capable and low-pressure.

Prefer:
- "Hide this item from guests"
- "Add an item"
- "Save changes"
- "Share registry"
- "Guests won't see disabled items."
- "Add a brand as a reference. Guests can still choose a similar product."

Avoid:
- "Unlock the power of a beautifully personalized registry experience"
- "Take full control of your gifting journey"
- "Elevate your baby's registry"

### Guest-facing

Guests should understand the registry without feeling ordered to buy something.

Prefer:
- "Puji added this as a reference."
- "Choose this gift"
- "Reserved"
- "Want to chip in? Any amount helps."
- "You don't have to buy the exact brand listed."

Avoid:
- fake urgency such as "Grab it before someone else does!"
- guilt such as "Help make baby's dreams come true"
- pressure such as "This is a must-have"
- implying a brand is medically or objectively best without evidence

### Empty states

Say what is empty and what the user can do next.

Prefer:
- "No items yet. Add the first one."
- "Nothing in Feeding yet."
- "All gifts in this category are currently hidden."

Avoid cute filler that makes the user decode the state.

## Patterns we remove

### Throat-clearing

Cut openers such as:
- "Here's the thing"
- "Let's dive in"
- "It's worth noting"
- "When it comes to"

State the point.

### Fake insight

Avoid:
- "What most parents don't realize..."
- "The part everyone misses..."
- "Here's what nobody tells you..."

If we have a useful fact, say the fact.

### Binary drama

Avoid the template:
- "It's not just a registry. It's a celebration of love."

Say what the product does.

### Importance puffery

Avoid:
- "game changer"
- "transformative"
- "pivotal"
- "revolutionary"
- "cutting-edge"
- "robust"
- "seamless" unless describing an observed interaction precisely

### Fake-profound endings

Do not end pages or modals with inspirational mic-drop lines. End with the next useful action or the actual information.

### Interpretive commentary

Avoid telling the reader how to feel:
- "The best part is..."
- "This is important."
- "As you can see..."
- "You'll love..."

Show the feature or consequence instead.

### Weasel claims

Do not write:
- "Experts recommend"
- "Parents love"
- "Studies show"
- "Most moms prefer"

unless the product actually has a named, relevant source and the claim belongs in the UI.

### Colon reveals

Do not use a colon to manufacture drama.

Bad:
"One thing to remember: disabled gifts disappear."

Better:
"Disabled gifts won't appear to guests."

Colons are fine for labels, lists, data, and ordinary grammar.

### Robotic rhythm

Do not stack lots of equally short fragments or make every card use the exact same sentence pattern. Consistency belongs in labels and controls; prose can breathe.

### Synonym cycling

Repeat the clearest product term. Consistency beats thesaurus variety.

### Decorative formatting

Avoid:
- emoji in functional headings
- random bold words inside sentences
- a heading for every two sentences
- bullet lists when one short paragraph reads better
- excessive em dashes

Emoji can appear as small visual accents in the registry design, especially item/category illustrations, but must not carry meaning by themselves.

## Words and phrases to avoid

Unless they are part of user-provided content, quotations, or a genuinely necessary technical term:

delve, foster, leverage, utilize, facilitate, empower, streamline, robust, cutting-edge, paradigm shift, game changer, tapestry, realm, beacon, multifaceted, meticulous, intricate, paramount, transformative, elevate, embark, supercharge, harness, ever-evolving.

Also remove empty filler such as:
"at the end of the day", "in today's world", "at its core", "the reality is", "in order to", "going forward", "let's dive in".

## Product-specific rules

### Buttons

Use action + object when context is not obvious.

Good:
- Add item
- Save profile
- Reserve gift
- Cancel reservation
- Copy guest link
- Hide from guests

Avoid:
- Continue
- Proceed
- Submit
- Let's go
- Make it happen

unless the surrounding flow makes the result unmistakable.

### Errors

Say what happened and, when known, how to fix it.

Good:
- "This gift was just reserved by someone else."
- "That slug is already in use. Try another one."
- "We couldn't save the item. Your changes are still here."

Do not blame the user. Do not add fake cheerfulness to errors.

### Confirmation

Confirm the completed action, not the interface action.

Good:
- "Item added."
- "Registry is now public."
- "Gift reserved for Dita."

Avoid:
- "Success!"
- "Amazing!"
- "Woohoo! Your operation was completed successfully!"

### Safety and baby-product copy

Do not turn generic registry guidance into medical advice.

For age-, weight-, sleep-, feeding-, or car-safety-dependent products:
- show model-specific limitations when we know them;
- otherwise say the parent/guest should check the manufacturer's current age, weight, installation, or use guidance;
- do not label a product "safe", "newborn-safe", "doctor recommended", or "best" without a verified basis.

### Prices and brands

Brands are examples, not endorsements.

Price ranges should include a date/source in editorial or admin data when practical. The guest UI can stay clean, but we should not present stale scraped prices as guaranteed current prices.

### Patungan

For expensive items, "patungan" should be clear and optional.

Prefer:
- "Patungan"
- "Contribute any amount"
- "Rp650.000 of Rp2.000.000 collected"

Do not use fundraising pressure or artificial progress language.

## Design copy hierarchy

A page should normally have:
1. one clear page title;
2. one short explanation only when needed;
3. the primary action;
4. content.

Do not add a kicker, subtitle, helper paragraph, banner, and tip when one sentence is enough.

Registry cards should prioritize:
1. item name;
2. price or contribution state;
3. useful parent note;
4. reference brand/model when present;
5. reservation state/action.

## Pre-merge copy check

Before shipping user-facing copy, ask:

- Does this tell the user something specific?
- Could this sentence be pasted into any unrelated app unchanged? If yes, make it specific or delete it.
- Did we invent a claim or emotion?
- Is one concept called by one consistent name?
- Is the button clear about what will happen?
- Can a sentence be shorter without losing personality?
- Are we using hype where a fact would work?
- Does Indonesian sound like a person in Indonesia would actually say it?
- Are cute elements helping the experience rather than hiding information?
- For baby/safety content, are we avoiding unsupported safety or medical claims?

If any answer is bad, fix the copy before merging.

## Reference

Adapted from Peter Yang's no-ai-slop project:
https://github.com/petergyang/no-ai-slop

Original concepts used here include preserving voice, minimum effective editing, concrete language, the portability test, active voice, cutting throat-clearing, fake insight, puffery, weasel attribution, synonym cycling, fake-profound endings, robotic rhythm, formatting slop, and unnecessary em dashes.

Little Registry adds product-specific rules for UI controls, Indonesian tone, guest/parent flows, registry brands/prices, patungan, and baby-product safety copy.
