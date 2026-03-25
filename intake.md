---
layout: default
title: Intake
permalink: /start-intake/
lang_alt_url: /formulario/
---

<article class="post intake-page">
  <header class="intake-hero">
    <p class="eyebrow">MESLO INTAKE</p>
    <h1 class="pageTitle">Tell us where your business stands right now.</h1>
    <p class="intro">
      Complete the intake form below so we can understand your current
      estimating process, operating constraints, and what kind of support makes
      the most sense.
    </p>
  </header>

  <form
    name="meslo-intake"
    method="POST"
    action="{{ '/start-intake/thanks/' | relative_url }}"
    data-netlify="true"
    netlify-honeypot="bot-field"
    class="intake-form"
  >
    <input type="hidden" name="form-name" value="meslo-intake">
    <p class="hidden-field">
      <label>Don't fill this out if you're human: <input name="bot-field"></label>
    </p>

    <section class="intake-section">
      <h2>1. Basic Info</h2>
      <div class="intake-grid intake-grid-2">
        <div class="field">
          <label for="full-name">Full Name</label>
          <input id="full-name" name="Full Name" type="text" required>
        </div>
        <div class="field">
          <label for="email">Email</label>
          <input id="email" name="Email" type="email" required>
        </div>
        <div class="field">
          <label for="phone-number">Phone Number</label>
          <input id="phone-number" name="Phone Number" type="text" required>
        </div>
        <div class="field">
          <label for="company-name">Company Name</label>
          <input id="company-name" name="Company Name" type="text" required>
        </div>
      </div>
    </section>

    <section class="intake-section">
      <h2>2. Business Snapshot</h2>
      <div class="field">
        <fieldset>
          <legend>What type of work do you primarily do?</legend>
          <label><input type="radio" name="Primary Work Type" value="General Contractor" required> General Contractor</label>
          <label><input type="radio" name="Primary Work Type" value="Subcontractor"> Subcontractor (HVAC, Electrical, Plumbing, etc.)</label>
          <label><input type="radio" name="Primary Work Type" value="Service Business"> Service Business</label>
          <label><input type="radio" name="Primary Work Type" value="Product Business"> Product Business</label>
          <label><input type="radio" name="Primary Work Type" value="Other"> Other</label>
          <input name="Primary Work Type Other" type="text" placeholder="If other, specify">
        </fieldset>
      </div>

      <div class="field">
        <fieldset>
          <legend>What is your average job size?</legend>
          <label><input type="radio" name="Average Job Size" value="Under $10K" required> Under $10K</label>
          <label><input type="radio" name="Average Job Size" value="$10K - $50K"> $10K - $50K</label>
          <label><input type="radio" name="Average Job Size" value="$50K - $250K"> $50K - $250K</label>
          <label><input type="radio" name="Average Job Size" value="$250K+"> $250K+</label>
        </fieldset>
      </div>

      <div class="field">
        <fieldset>
          <legend>What is your current monthly revenue?</legend>
          <label><input type="radio" name="Current Monthly Revenue" value="Under $50K" required> Under $50K</label>
          <label><input type="radio" name="Current Monthly Revenue" value="$50K - $150K"> $50K - $150K</label>
          <label><input type="radio" name="Current Monthly Revenue" value="$150K - $500K"> $150K - $500K</label>
          <label><input type="radio" name="Current Monthly Revenue" value="$500K+"> $500K+</label>
        </fieldset>
      </div>
    </section>

    <section class="intake-section">
      <h2>3. Current State</h2>
      <div class="field">
        <fieldset>
          <legend>How are you currently estimating your jobs?</legend>
          <label><input type="radio" name="Current Estimating Method" value="Spreadsheet" required> Spreadsheet</label>
          <label><input type="radio" name="Current Estimating Method" value="Pen & paper"> Pen &amp; paper</label>
          <label><input type="radio" name="Current Estimating Method" value="Software"> Software (please specify)</label>
          <label><input type="radio" name="Current Estimating Method" value="No consistent system"> No consistent system</label>
          <input name="Estimating Software" type="text" placeholder="If software, specify">
        </fieldset>
      </div>

      <div class="field">
        <fieldset>
          <legend>Do you know your true overhead and profit targets?</legend>
          <label><input type="radio" name="Overhead and Profit Clarity" value="Yes, clearly" required> Yes, clearly</label>
          <label><input type="radio" name="Overhead and Profit Clarity" value="Somewhat"> Somewhat</label>
          <label><input type="radio" name="Overhead and Profit Clarity" value="No"> No</label>
        </fieldset>
      </div>
    </section>

    <section class="intake-section">
      <h2>4. Problem Identification</h2>
      <div class="field">
        <fieldset>
          <legend>What is your biggest issue right now? (Select all that apply)</legend>
          <label><input type="checkbox" name="Biggest Issues" value="Underbidding jobs"> Underbidding jobs</label>
          <label><input type="checkbox" name="Biggest Issues" value="Not knowing true costs"> Not knowing true costs</label>
          <label><input type="checkbox" name="Biggest Issues" value="Inconsistent estimating"> Inconsistent estimating</label>
          <label><input type="checkbox" name="Biggest Issues" value="Cash flow issues"> Cash flow issues</label>
          <label><input type="checkbox" name="Biggest Issues" value="Too much manual work"> Too much manual work</label>
          <label><input type="checkbox" name="Biggest Issues" value="No clear systems"> No clear systems</label>
          <label><input type="checkbox" name="Biggest Issues" value="Scaling problems"> Scaling problems</label>
        </fieldset>
      </div>

      <div class="field">
        <label for="main-problem">In one sentence, what’s the main problem you want to fix?</label>
        <textarea id="main-problem" name="Main Problem to Fix" required></textarea>
      </div>
    </section>

    <section class="intake-section">
      <h2>5. Desired Outcome</h2>
      <div class="field">
        <label for="success-90-days">What would success look like in the next 90 days?</label>
        <textarea id="success-90-days" name="90 Day Success Definition" required></textarea>
      </div>
    </section>

    <section class="intake-section">
      <h2>6. Readiness Filter</h2>
      <div class="field">
        <fieldset>
          <legend>Are you looking for:</legend>
          <label><input type="radio" name="What They Are Looking For" value="A system I can implement myself" required> A system I can implement myself</label>
          <label><input type="radio" name="What They Are Looking For" value="Guidance on real jobs"> Guidance on real jobs</label>
          <label><input type="radio" name="What They Are Looking For" value="Someone to help build systems with me"> Someone to help build systems with me</label>
          <label><input type="radio" name="What They Are Looking For" value="Full operational support"> Full operational support</label>
        </fieldset>
      </div>

      <div class="field">
        <fieldset>
          <legend>Are you prepared to invest in improving your estimating and operational systems?</legend>
          <label><input type="radio" name="Investment Readiness" value="Yes" required> Yes</label>
          <label><input type="radio" name="Investment Readiness" value="Maybe"> Maybe</label>
          <label><input type="radio" name="Investment Readiness" value="No"> No</label>
        </fieldset>
      </div>
    </section>

    <section class="intake-section">
      <h2>7. Positioning Question</h2>
      <div class="field">
        <label for="business-impact">If we could fix your estimating and pricing, what impact would that have on your business?</label>
        <textarea id="business-impact" name="Business Impact of Better Estimating and Pricing" required></textarea>
      </div>
    </section>

    <div class="intake-actions">
      <button class="button" type="submit">Submit Intake Form</button>
    </div>
  </form>
</article>
