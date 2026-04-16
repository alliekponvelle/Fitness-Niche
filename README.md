<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Module 18 - Fitness Niche | The Creator Plug Academy</title>
  <style>
    :root {
      --ink: #24192f;
      --muted: #6f6178;
      --panel: #ffffff;
      --gold: #d9a441;
      --gold-soft: #fff2c9;
      --rose: #f05d8a;
      --teal: #18a6a7;
      --violet: #4d2770;
      --violet-deep: #241332;
      --line: #eadfce;
      --shadow: 0 18px 40px rgba(48, 31, 61, 0.14);
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      color: var(--ink);
      background:
        radial-gradient(circle at 14% 8%, rgba(240, 93, 138, 0.15), transparent 28%),
        radial-gradient(circle at 88% 4%, rgba(24, 166, 167, 0.16), transparent 26%),
        linear-gradient(180deg, #fffaf1 0%, #f8f1e7 45%, #f4ebdd 100%);
      line-height: 1.6;
    }
    a { color: #2c6f91; font-weight: 800; }
    .page { width: min(1120px, calc(100% - 32px)); margin: 0 auto; padding: 28px 0 56px; }
    .hero { background: linear-gradient(135deg, rgba(36, 19, 50, 0.96), rgba(77, 39, 112, 0.92)); color: #fff; border-radius: 8px; padding: 34px; box-shadow: var(--shadow); position: relative; overflow: hidden; }
    .hero:after { content: ""; position: absolute; right: -78px; top: -82px; width: 260px; height: 260px; border: 2px solid rgba(217, 164, 65, 0.36); transform: rotate(20deg); }
    .eyebrow { display: inline-flex; background: rgba(217, 164, 65, 0.18); border: 1px solid rgba(217, 164, 65, 0.45); color: #ffe3a0; border-radius: 8px; padding: 7px 11px; font-size: 13px; font-weight: 800; letter-spacing: 0.08em; text-transform: uppercase; }
    h1, h2, h3 { line-height: 1.15; margin: 0; }
    h1 { max-width: 880px; margin-top: 18px; font-size: clamp(34px, 6vw, 70px); }
    .subtitle { max-width: 860px; margin: 18px 0 0; color: #f6e9d6; font-size: 18px; }
    .quick-links { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 24px; position: relative; z-index: 1; }
    .quick-links a, .button-link, .copy-button { appearance: none; border: 0; border-radius: 8px; background: var(--gold); color: #241332; cursor: pointer; display: inline-flex; align-items: center; justify-content: center; font-family: inherit; font-size: 14px; font-weight: 900; line-height: 1; min-height: 42px; padding: 12px 14px; text-decoration: none; }
    .quick-links a:hover, .button-link:hover, .copy-button:hover { background: #f1c761; }
    .button-link.secondary { background: #ffffff; border: 1px solid var(--line); color: var(--violet); }
    .hero-grid, .three-col { display: grid; grid-template-columns: repeat(3, 1fr); gap: 14px; margin-top: 26px; }
    .hero-card { background: rgba(255, 255, 255, 0.1); border: 1px solid rgba(255, 255, 255, 0.18); border-radius: 8px; padding: 18px; min-height: 126px; }
    .hero-card strong { color: #ffe1a1; display: block; font-size: 15px; text-transform: uppercase; letter-spacing: 0.08em; margin-bottom: 8px; }
    .section { margin-top: 24px; background: rgba(255, 255, 255, 0.88); border: 1px solid var(--line); border-radius: 8px; padding: 28px; box-shadow: 0 10px 24px rgba(48, 31, 61, 0.08); }
    .section h2 { color: var(--violet-deep); font-size: clamp(25px, 3vw, 38px); margin-bottom: 12px; }
    .section-intro { max-width: 900px; color: var(--muted); margin: 0 0 20px; }
    .two-col { display: grid; grid-template-columns: repeat(2, 1fr); gap: 16px; }
    .card { background: var(--panel); border: 1px solid var(--line); border-radius: 8px; padding: 20px; }
    .card h3 { color: var(--violet); font-size: 20px; margin-bottom: 8px; }
    .tag { display: inline-block; border-radius: 8px; padding: 5px 9px; margin-bottom: 12px; background: var(--gold-soft); color: #765210; font-weight: 800; font-size: 12px; text-transform: uppercase; letter-spacing: 0.06em; }
    ul, ol { margin: 10px 0 0 20px; padding: 0; }
    li { margin: 8px 0; }
    .link-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 12px; margin-bottom: 24px; }
    .lesson-link { background: #fff; border: 1px solid var(--line); border-radius: 8px; color: var(--violet-deep); display: block; font-weight: 800; padding: 14px; text-decoration: none; }
    .lesson-link:hover { border-color: var(--gold); box-shadow: 0 8px 20px rgba(48, 31, 61, 0.1); transform: translateY(-1px); }
    .lesson { display: grid; grid-template-columns: 84px 1fr; gap: 16px; border-top: 1px solid var(--line); padding: 20px 0; }
    .lesson:first-of-type { border-top: 0; padding-top: 0; }
    .lesson-number { width: 64px; height: 64px; border-radius: 8px; background: linear-gradient(135deg, var(--violet), var(--rose)); color: #fff; display: grid; place-items: center; font-size: 24px; font-weight: 900; box-shadow: 0 12px 22px rgba(77, 39, 112, 0.22); }
    .lesson-number a { color: #fff; display: grid; height: 100%; place-items: center; text-decoration: none; width: 100%; }
    .callout { border-left: 5px solid var(--gold); background: #fff7dc; padding: 16px 18px; border-radius: 8px; margin-top: 16px; }
    .warning { border-left-color: var(--rose); background: #fff0f5; }
    table { width: 100%; border-collapse: collapse; overflow: hidden; border-radius: 8px; background: #fff; border: 1px solid var(--line); }
    th, td { text-align: left; vertical-align: top; border-bottom: 1px solid var(--line); padding: 14px; }
    th { background: var(--violet-deep); color: #fff; font-size: 13px; text-transform: uppercase; letter-spacing: 0.06em; }
    tr:last-child td { border-bottom: 0; }
    .script-box { background: #241332; color: #fdf5e8; border-radius: 8px; padding: 18px; font-family: "Courier New", Courier, monospace; font-size: 14px; line-height: 1.55; white-space: pre-wrap; }
    .copy-row { align-items: center; display: flex; flex-wrap: wrap; gap: 10px; justify-content: space-between; margin-bottom: 10px; }
    .checklist { list-style: none; margin-left: 0; }
    .checklist li { padding-left: 34px; position: relative; }
    .checklist li:before { content: ""; position: absolute; left: 0; top: 5px; width: 19px; height: 19px; border-radius: 5px; border: 2px solid var(--teal); background: #efffff; }
    .footer { margin-top: 24px; text-align: center; color: var(--muted); font-size: 14px; }
    @media (max-width: 820px) {
      .hero { padding: 24px; }
      .hero-grid, .two-col, .three-col, .link-grid { grid-template-columns: 1fr; }
      .lesson { grid-template-columns: 1fr; }
      table, thead, tbody, th, td, tr { display: block; }
      th { display: none; }
      td { border-bottom: 0; padding: 12px 14px; }
      tr { border-bottom: 1px solid var(--line); padding: 8px 0; }
    }
  </style>
</head>
<body>
  <main class="page" id="top">
    <section class="hero">
      <span class="eyebrow">The Creator Plug Academy - Module 18</span>
      <h1>Fitness Niche</h1>
      <p class="subtitle">
        A monetization module for creators who want to build a fitness or wellness niche through content, digital products, templates, coaching, affiliate offers, and safe audience education.
      </p>
      <nav class="quick-links" aria-label="Module quick links">
        <a href="#overview">Overview</a>
        <a href="#lessons">Lessons</a>
        <a href="#offers">Offers</a>
        <a href="#content">Content</a>
        <a href="#templates">Templates</a>
        <a href="#affiliate">Affiliate</a>
        <a href="#challenge">Challenge</a>
        <a href="#sources">Sources</a>
      </nav>
      <div class="hero-grid">
        <div class="hero-card"><strong>Best For</strong>Creators in fitness, wellness, weight loss, strength, home workouts, routines, meal prep, or accountability niches.</div>
        <div class="hero-card"><strong>Core Skill</strong>Turning fitness knowledge and lifestyle content into safe, useful, monetizable offers without making risky health claims.</div>
        <div class="hero-card"><strong>Final Outcome</strong>A fitness niche plan with content pillars, offer ideas, disclaimers, digital products, affiliate strategy, and launch checklist.</div>
      </div>
    </section>

    <section class="section" id="overview">
      <h2>Module Overview</h2>
      <p class="section-intro">
        Fitness is a strong niche because people want support with routines, confidence, energy, strength, weight management, meal planning, and accountability. But it is also a sensitive niche because creators can easily cross into medical advice, unsafe promises, body-shaming, or unsupported supplement claims. This module teaches students how to build a fitness income stream responsibly.
      </p>
      <div class="two-col">
        <div class="card">
          <span class="tag">What students learn</span>
          <ul>
            <li>How to choose a fitness niche and audience.</li>
            <li>How to create safe fitness content pillars.</li>
            <li>How to sell planners, trackers, workout templates, coaching, and challenges.</li>
            <li>How to use disclaimers and avoid medical or supplement claims.</li>
            <li>How to build affiliate income without promoting random products.</li>
          </ul>
        </div>
        <div class="card">
          <span class="tag">Safety boundary</span>
          <p>
            This module is for business education. Students should not diagnose, treat, cure, or prevent disease. They should not create personalized exercise or nutrition plans outside their qualifications. Encourage audiences to consult qualified professionals when needed.
          </p>
        </div>
      </div>
      <div class="callout warning">
        <strong>Health claim rule:</strong> Any fitness, nutrition, supplement, or transformation claim needs to be truthful, not misleading, and supported. Do not promise specific weight loss, body changes, or health outcomes.
      </div>
    </section>

    <section class="section" id="lessons">
      <h2>Full Lesson Plan</h2>
      <p class="section-intro">This curriculum teaches the fitness niche as a business model: content, community, products, coaching, affiliate income, and safety.</p>
      <div class="link-grid">
        <a class="lesson-link" href="#lesson-1">1. Pick a Fitness Lane</a>
        <a class="lesson-link" href="#lesson-2">2. Define the Audience</a>
        <a class="lesson-link" href="#lesson-3">3. Build Content Pillars</a>
        <a class="lesson-link" href="#lesson-4">4. Create Digital Fitness Products</a>
        <a class="lesson-link" href="#lesson-5">5. Build a Fitness Challenge</a>
        <a class="lesson-link" href="#lesson-6">6. Offer Coaching Safely</a>
        <a class="lesson-link" href="#lesson-7">7. Affiliate Products</a>
        <a class="lesson-link" href="#lesson-8">8. Transformation Content</a>
        <a class="lesson-link" href="#lesson-9">9. Claims, Disclaimers, and Boundaries</a>
        <a class="lesson-link" href="#lesson-10">10. Launch the Fitness Offer</a>
      </div>

      <div class="lesson" id="lesson-1">
        <div class="lesson-number"><a href="#lessons">1</a></div>
        <div>
          <h3>Pick a Fitness Lane</h3>
          <p>A fitness lane keeps the brand focused. Students should choose a lane based on experience, audience needs, and what they can talk about consistently.</p>
          <div class="three-col">
            <div class="card"><h3>Beginner Fitness</h3><p>For people starting from low confidence, no routine, or gym anxiety.</p></div>
            <div class="card"><h3>Home Workouts</h3><p>For busy people who want simple workouts without a gym.</p></div>
            <div class="card"><h3>Strength Training</h3><p>For people who want to get stronger and learn form basics.</p></div>
            <div class="card"><h3>Wellness Routines</h3><p>For habits, energy, walking, stretching, hydration, sleep, and consistency.</p></div>
            <div class="card"><h3>Meal Prep</h3><p>For planning meals, grocery lists, prep routines, and simple nutrition education.</p></div>
            <div class="card"><h3>Accountability</h3><p>For challenges, check-ins, community, habit tracking, and motivation.</p></div>
          </div>
        </div>
      </div>

      <div class="lesson" id="lesson-2">
        <div class="lesson-number"><a href="#lessons">2</a></div>
        <div>
          <h3>Define the Audience</h3>
          <p>The fitness niche gets stronger when the creator speaks to one person with one problem. "Fitness for everyone" is too broad.</p>
          <div class="script-box">Audience worksheet:
My fitness content helps:
___

They struggle with:
___

They want to feel:
___

They need support with:
___

They are not looking for:
___

My safe promise is:
___</div>
          <div class="callout"><strong>Example:</strong> "I help busy moms build a simple 20-minute home workout routine without gym pressure or extreme dieting."</div>
        </div>
      </div>

      <div class="lesson" id="lesson-3">
        <div class="lesson-number"><a href="#lessons">3</a></div>
        <div>
          <h3>Build Content Pillars</h3>
          <p>Fitness content should educate, motivate, demonstrate, and build trust. Students should rotate pillars so the account does not become only transformation posts or random workouts.</p>
          <table>
            <thead><tr><th>Pillar</th><th>Purpose</th><th>Post Ideas</th></tr></thead>
            <tbody>
              <tr><td>Education</td><td>Teach safe basics.</td><td>form tips, beginner mistakes, recovery, warmups, habit building</td></tr>
              <tr><td>Demonstration</td><td>Show the movement or routine.</td><td>3-move home workout, beginner stretch flow, meal prep demo</td></tr>
              <tr><td>Motivation</td><td>Build consistency and identity.</td><td>mindset reminders, small wins, realistic routines</td></tr>
              <tr><td>Proof</td><td>Show process without misleading.</td><td>your routine, client wins with permission, challenge completion</td></tr>
              <tr><td>Offer</td><td>Invite buyers to the next step.</td><td>planner promo, challenge invite, coaching waitlist, affiliate tutorial</td></tr>
            </tbody>
          </table>
        </div>
      </div>

      <div class="lesson" id="lesson-4">
        <div class="lesson-number"><a href="#lessons">4</a></div>
        <div>
          <h3>Create Digital Fitness Products</h3>
          <p>Fitness creators can monetize before they are ready for coaching by selling planners, trackers, guides, and templates.</p>
          <div class="three-col">
            <div class="card"><h3>Workout Planner</h3><p>Weekly workout schedule, movement tracker, progress log, and reflection pages.</p></div>
            <div class="card"><h3>Meal Prep Planner</h3><p>Meal ideas, grocery list, prep schedule, pantry list, and weekly review.</p></div>
            <div class="card"><h3>Habit Tracker</h3><p>Steps, water, sleep, workouts, stretching, protein goals, and mood tracking.</p></div>
            <div class="card"><h3>Challenge Workbook</h3><p>7-day, 14-day, or 30-day challenge with daily checklists and prompts.</p></div>
            <div class="card"><h3>Fitness Journal</h3><p>Mindset, confidence, body-neutral reflection, consistency notes, and wins.</p></div>
            <div class="card"><h3>Template Bundle</h3><p>Canva social posts, challenge graphics, tracker pages, and content calendar.</p></div>
          </div>
        </div>
      </div>

      <div class="lesson" id="lesson-5">
        <div class="lesson-number"><a href="#lessons">5</a></div>
        <div>
          <h3>Build a Fitness Challenge</h3>
          <p>A challenge is a strong beginner offer because it gives structure and urgency. The best challenges focus on actions the participant can control.</p>
          <table>
            <thead><tr><th>Challenge Type</th><th>Good Promise</th><th>Avoid Saying</th></tr></thead>
            <tbody>
              <tr><td>7-Day Walk Challenge</td><td>Build a daily walking routine.</td><td>Lose 10 pounds in a week.</td></tr>
              <tr><td>14-Day Home Workout Challenge</td><td>Complete simple beginner workouts at home.</td><td>Guaranteed body transformation.</td></tr>
              <tr><td>30-Day Consistency Challenge</td><td>Track movement, hydration, and recovery habits.</td><td>Fix your health forever.</td></tr>
            </tbody>
          </table>
        </div>
      </div>

      <div class="lesson" id="lesson-6">
        <div class="lesson-number"><a href="#lessons">6</a></div>
        <div>
          <h3>Offer Coaching Safely</h3>
          <p>Fitness coaching can be powerful, but students need boundaries. Coaches should operate within their qualifications, avoid medical advice, and use intake forms to understand risk factors.</p>
          <ul class="checklist">
            <li>Use an intake form before coaching.</li>
            <li>Ask about injuries, limitations, and medical concerns.</li>
            <li>Encourage clients to consult a qualified professional when needed.</li>
            <li>Do not prescribe diets unless properly qualified.</li>
            <li>Do not promise specific weight loss or health outcomes.</li>
            <li>Keep client records organized.</li>
            <li>Use a coaching agreement and liability disclaimer.</li>
          </ul>
        </div>
      </div>

      <div class="lesson" id="lesson-7">
        <div class="lesson-number"><a href="#lessons">7</a></div>
        <div>
          <h3>Affiliate Products</h3>
          <p>Fitness affiliate income should match the creator's actual routine and audience. Students should only recommend products they understand and can explain honestly.</p>
          <div class="three-col">
            <div class="card"><h3>Low-Risk Ideas</h3><ul><li>water bottles</li><li>resistance bands</li><li>yoga mats</li><li>meal prep containers</li><li>journals</li><li>workout timers</li></ul></div>
            <div class="card"><h3>Higher-Caution Ideas</h3><ul><li>supplements</li><li>fat burners</li><li>detox teas</li><li>medical devices</li><li>extreme programs</li><li>injury tools</li></ul></div>
            <div class="card"><h3>Review Before Promoting</h3><ul><li>claims</li><li>refunds</li><li>reviews</li><li>ingredients</li><li>audience fit</li><li>affiliate disclosure</li></ul></div>
          </div>
        </div>
      </div>

      <div class="lesson" id="lesson-8">
        <div class="lesson-number"><a href="#lessons">8</a></div>
        <div>
          <h3>Transformation Content</h3>
          <p>Transformation content can be powerful, but it must be truthful and not misleading. Students should focus on process, habits, and lived experience instead of making every post about body comparison.</p>
          <div class="two-col">
            <div class="card"><h3>Better Angles</h3><ul><li>what changed in my routine</li><li>how I built consistency</li><li>mistakes I stopped making</li><li>what I track now</li><li>how I rest and recover</li></ul></div>
            <div class="card"><h3>Avoid</h3><ul><li>guaranteed outcomes</li><li>extreme before/after claims</li><li>body shaming</li><li>using someone else's photo</li><li>hiding important context</li></ul></div>
          </div>
        </div>
      </div>

      <div class="lesson" id="lesson-9">
        <div class="lesson-number"><a href="#lessons">9</a></div>
        <div>
          <h3>Claims, Disclaimers, and Boundaries</h3>
          <p>Disclaimers do not fix false claims, but they help set expectations. The claim itself still needs to be truthful and supported.</p>
          <div class="script-box">Simple disclaimer:
This content is for educational and informational purposes only. It is not medical advice. Always consult a qualified healthcare professional before starting a new fitness, nutrition, or supplement routine, especially if you have injuries, medical conditions, or concerns.</div>
        </div>
      </div>

      <div class="lesson" id="lesson-10">
        <div class="lesson-number"><a href="#lessons">10</a></div>
        <div>
          <h3>Launch the Fitness Offer</h3>
          <p>Students should launch with one focused offer and a simple content path: teach the problem, show the routine, invite people to the product or challenge, and collect feedback.</p>
          <ol>
            <li>Choose one audience and one offer.</li>
            <li>Create 10 educational posts.</li>
            <li>Create 5 demonstration posts.</li>
            <li>Create 3 story/proof posts.</li>
            <li>Create 3 invitation posts.</li>
            <li>Launch the product, challenge, or coaching waitlist.</li>
          </ol>
        </div>
      </div>
    </section>

    <section class="section" id="offers">
      <h2>Fitness Offer Menu</h2>
      <p class="section-intro">Students can choose one offer type to start. The goal is to validate a simple product before building a whole fitness brand empire.</p>
      <table>
        <thead><tr><th>Offer</th><th>Includes</th><th>Best First Price Range</th></tr></thead>
        <tbody>
          <tr><td>Fitness Tracker PDF</td><td>workouts, steps, water, sleep, habit tracking</td><td>$5-$15</td></tr>
          <tr><td>30-Day Challenge Workbook</td><td>daily actions, checklists, reflection, progress log</td><td>$17-$37</td></tr>
          <tr><td>Meal Prep Planner</td><td>grocery list, prep schedule, meal ideas, pantry list</td><td>$9-$29</td></tr>
          <tr><td>Beginner Workout Guide</td><td>simple routines, warmup, cooldown, tracker</td><td>$17-$47</td></tr>
          <tr><td>Group Accountability Challenge</td><td>community, check-ins, habit tracking, weekly calls</td><td>$27-$97</td></tr>
          <tr><td>Fitness Content Template Pack</td><td>Canva posts, trackers, challenge graphics, captions</td><td>$17-$67</td></tr>
        </tbody>
      </table>
    </section>

    <section class="section" id="content">
      <h2>Fitness Content Prompts</h2>
      <div class="three-col">
        <div class="card"><h3>Education Prompts</h3><ol><li>3 beginner workout mistakes</li><li>how to warm up before a home workout</li><li>how to make walking more consistent</li><li>why rest days matter</li><li>how to start when you feel out of shape</li></ol></div>
        <div class="card"><h3>Demo Prompts</h3><ol><li>3-move no-equipment workout</li><li>5-minute stretch routine</li><li>meal prep container setup</li><li>how to track workouts</li><li>beginner band workout</li></ol></div>
        <div class="card"><h3>Offer Prompts</h3><ol><li>what is inside my 30-day challenge</li><li>who this tracker is for</li><li>how to use the planner</li><li>why I created this workbook</li><li>join the challenge if you need accountability</li></ol></div>
      </div>
    </section>

    <section class="section" id="templates">
      <h2>Copy-Ready Templates</h2>
      <div class="two-col">
        <div class="card">
          <div class="copy-row"><h3>Fitness Offer Description</h3><button class="copy-button" type="button" data-copy-target="fitness-description">Copy Template</button></div>
          <div class="script-box" id="fitness-description">This ___ was created for ___ who want to build a more consistent fitness routine without ___.

Inside, you will get:
- ___
- ___
- ___

Use this to:
- plan ___
- track ___
- stay consistent with ___

This is educational content, not medical advice. Please consult a qualified professional before beginning a new fitness or nutrition routine.</div>
        </div>
        <div class="card">
          <div class="copy-row"><h3>Challenge Invite</h3><button class="copy-button" type="button" data-copy-target="challenge-invite">Copy Invite</button></div>
          <div class="script-box" id="challenge-invite">I am starting a ___ day challenge for ___ who want to ___.

This is not about being perfect. It is about building consistency with simple daily actions.

You will get:
- ___
- ___
- ___

Comment ___ or click the link in my bio if you want the details.</div>
        </div>
        <div class="card">
          <div class="copy-row"><h3>Affiliate Disclosure</h3><button class="copy-button" type="button" data-copy-target="affiliate-disclosure">Copy Disclosure</button></div>
          <div class="script-box" id="affiliate-disclosure">Disclosure: This post may contain affiliate links. If you purchase through my link, I may earn a commission at no extra cost to you. I only share products I believe may be helpful for my audience.</div>
        </div>
        <div class="card">
          <div class="copy-row"><h3>Client Intake Questions</h3><button class="copy-button" type="button" data-copy-target="fitness-intake">Copy Questions</button></div>
          <div class="script-box" id="fitness-intake">1. What is your main fitness goal right now?
2. What is your current activity level?
3. Do you have any injuries, limitations, or medical concerns?
4. Are you cleared by a qualified professional to exercise?
5. What equipment do you have access to?
6. How many days per week can you realistically commit?
7. What type of support do you need most?
8. What does success look like for you?</div>
        </div>
      </div>
    </section>

    <section class="section" id="affiliate">
      <h2>Affiliate Strategy</h2>
      <p class="section-intro">A good fitness affiliate strategy is built on trust. Students should only promote products that fit the audience and can be explained honestly.</p>
      <table>
        <thead><tr><th>Product Category</th><th>Content Angle</th><th>Safety Check</th></tr></thead>
        <tbody>
          <tr><td>Resistance bands</td><td>beginner home workout demo</td><td>show proper use and avoid overclaiming results</td></tr>
          <tr><td>Water bottle</td><td>hydration habit routine</td><td>do not imply it creates health outcomes by itself</td></tr>
          <tr><td>Meal prep containers</td><td>weekly prep setup</td><td>focus on organization, not medical nutrition claims</td></tr>
          <tr><td>Workout mat</td><td>home workout setup</td><td>explain comfort and use case honestly</td></tr>
          <tr><td>Supplements</td><td>only if qualified and carefully disclosed</td><td>avoid disease, weight-loss, or guaranteed outcome claims</td></tr>
        </tbody>
      </table>
    </section>

    <section class="section" id="challenge">
      <h2>14-Day Fitness Niche Launch Challenge</h2>
      <table>
        <thead><tr><th>Day</th><th>Assignment</th><th>Deliverable</th></tr></thead>
        <tbody>
          <tr><td>1</td><td>Choose one fitness lane.</td><td>Niche statement.</td></tr>
          <tr><td>2</td><td>Define audience and safe promise.</td><td>Audience worksheet.</td></tr>
          <tr><td>3</td><td>Create 4 content pillars.</td><td>Content pillar map.</td></tr>
          <tr><td>4</td><td>Choose one offer.</td><td>Offer outline.</td></tr>
          <tr><td>5</td><td>Create product page list or challenge plan.</td><td>Product outline.</td></tr>
          <tr><td>6</td><td>Write disclaimer and boundaries.</td><td>Safety copy.</td></tr>
          <tr><td>7</td><td>Create 5 educational posts.</td><td>Content drafts.</td></tr>
          <tr><td>8</td><td>Create 3 demo posts.</td><td>Video ideas.</td></tr>
          <tr><td>9</td><td>Create 3 offer posts.</td><td>CTA drafts.</td></tr>
          <tr><td>10</td><td>Choose 3 affiliate products to research.</td><td>Affiliate review notes.</td></tr>
          <tr><td>11</td><td>Create mockup or offer image.</td><td>Promo image.</td></tr>
          <tr><td>12</td><td>Write product description.</td><td>Sales copy.</td></tr>
          <tr><td>13</td><td>Publish one value post.</td><td>Posted content.</td></tr>
          <tr><td>14</td><td>Publish one offer invite.</td><td>Launch post.</td></tr>
        </tbody>
      </table>
    </section>

    <section class="section" id="mistakes">
      <h2>Beginner Mistakes to Avoid</h2>
      <div class="two-col">
        <div class="card"><h3>Making Unsafe Claims</h3><p>Do not promise specific weight loss, cures, or guaranteed health outcomes.</p></div>
        <div class="card"><h3>Body Shaming</h3><p>Fear-based content can damage trust. Focus on strength, habits, confidence, energy, and consistency.</p></div>
        <div class="card"><h3>Promoting Random Supplements</h3><p>Supplement claims are highly regulated and should be handled with extra care.</p></div>
        <div class="card"><h3>No Qualifications Boundary</h3><p>Be honest about certifications, experience, and what you are qualified to teach.</p></div>
        <div class="card"><h3>No Intake Process</h3><p>Fitness support needs intake questions so the creator understands limitations and risk.</p></div>
        <div class="card"><h3>Only Posting Workouts</h3><p>Mix workouts with education, mindset, routine building, proof, and offers.</p></div>
      </div>
    </section>

    <section class="section" id="completion">
      <h2>Module Completion Requirements</h2>
      <ul class="checklist">
        <li>Choose one fitness niche lane.</li>
        <li>Define audience, problem, and safe promise.</li>
        <li>Create 4 content pillars.</li>
        <li>Choose one first offer.</li>
        <li>Create an offer description and disclaimer.</li>
        <li>Draft 10 pieces of content.</li>
        <li>Research 3 affiliate products safely.</li>
        <li>Create a launch post and CTA.</li>
        <li>Review claims, disclaimers, and boundaries before publishing.</li>
      </ul>
    </section>

    <section class="section" id="sources">
      <h2>Official Reference Links</h2>
      <p class="section-intro">These sources help keep the module aligned with official health, advertising, and supplement-claim guidance.</p>
      <ul>
        <li><a href="https://health.gov/our-work/nutrition-physical-activity/physical-activity-guidelines" target="_blank" rel="noopener">HHS: Physical Activity Guidelines for Americans</a></li>
        <li><a href="https://www.cdc.gov/physical-activity-basics/guidelines/adults.html" target="_blank" rel="noopener">CDC: Adult Physical Activity Guidelines</a></li>
        <li><a href="https://www.ftc.gov/business-guidance/resources/health-products-compliance-guidance" target="_blank" rel="noopener">FTC: Health Products Compliance Guidance</a></li>
        <li><a href="https://www.fda.gov/food/dietary-supplements/dietary-supplement-labeling-guide-chapter-vi-claims" target="_blank" rel="noopener">FDA: Dietary Supplement Claims Guidance</a></li>
      </ul>
    </section>

    <p class="footer">
      <a class="button-link secondary" href="#top">Back to top</a>
      <br /><br />
      The Creator Plug Academy - Fitness Niche - April 2026
    </p>
  </main>
  <script>
    document.querySelectorAll("[data-copy-target]").forEach(function(button) {
      button.addEventListener("click", function() {
        var target = document.getElementById(button.getAttribute("data-copy-target"));
        if (!target) return;
        var text = target.innerText;
        var copyText = function() {
          var textArea = document.createElement("textarea");
          textArea.value = text;
          textArea.setAttribute("readonly", "");
          textArea.style.position = "fixed";
          textArea.style.left = "-9999px";
          document.body.appendChild(textArea);
          textArea.select();
          document.execCommand("copy");
          document.body.removeChild(textArea);
        };
        var copied = navigator.clipboard && window.isSecureContext
          ? navigator.clipboard.writeText(text)
          : new Promise(function(resolve) {
              copyText();
              resolve();
            });
        copied.then(function() {
          var original = button.innerText;
          button.innerText = "Copied";
          setTimeout(function() { button.innerText = original; }, 1600);
        });
      });
    });
  </script>
</body>
</html>
