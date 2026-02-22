---
layout: archive
permalink: temporary/home
title: ""
author_profile: false
---

<link href="https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500&family=Spectral:ital,wght@0,300;0,400;0,600;1,300;1,400&display=swap" rel="stylesheet" />

<style>
/* ── THEME VARIABLES ── */
:root {
  --ck-bg: #f9f7f3;
  --ck-text: #1a1a1a;
  --ck-text-muted: #444;
  --ck-accent: #8b1a1a;
  --ck-border: #d5cfc5;
  --ck-section-rule: #c9c3b8;
  --ck-tag-bg: #ede9e2;
  --ck-toggle-bg: #e2ddd6;
  --ck-link: #8b1a1a;
  --ck-link-hover: #5a1010;
}

[data-ck-theme="dark"] {
  --ck-bg: #141210;
  --ck-text: #e8e4dc;
  --ck-text-muted: #a09888;
  --ck-accent: #c97a5a;
  --ck-border: #2e2a26;
  --ck-section-rule: #2e2a26;
  --ck-tag-bg: #252118;
  --ck-toggle-bg: #2e2a26;
  --ck-link: #c97a5a;
  --ck-link-hover: #e09070;
}

/* scope everything under .ck-page to avoid clashing with MM styles */
.ck-page {
  background: var(--ck-bg);
  color: var(--ck-text);
  font-family: 'Spectral', Georgia, serif;
  font-weight: 300;
  line-height: 1.65;
  padding: 2.5rem 0 4rem;
  transition: background 0.3s, color 0.3s;
}

/* ── TOGGLE ── */
.ck-toggle {
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
  background: var(--ck-toggle-bg);
  border: 1px solid var(--ck-border);
  border-radius: 2rem;
  padding: 0.28rem 0.7rem;
  cursor: pointer;
  font-size: 0.77rem;
  letter-spacing: 0.08em;
  color: var(--ck-text-muted);
  font-family: 'Spectral', serif;
  margin-bottom: 2rem;
  transition: border-color 0.2s;
}
.ck-toggle:hover { border-color: var(--ck-accent); color: var(--ck-text); }
.ck-toggle-dot {
  width: 12px; height: 12px;
  border-radius: 50%;
  background: var(--ck-accent);
  display: inline-block;
}

/* ── GRID ── */
.ck-grid {
  display: grid;
  grid-template-columns: 300px 1fr;
  gap: 0 3.5rem;
}
@media (max-width: 720px) {
  .ck-grid { grid-template-columns: 1fr; }
  .ck-left { margin-bottom: 2.5rem; }
}

/* ── LEFT ── */
.ck-left { grid-column: 1; }

h1.ck-name {
  font-family: 'EB Garamond', Georgia, serif;
  font-size: 2.8rem;
  font-weight: 500;
  line-height: 1.1;
  color: var(--ck-text);
  margin: 0 0 0.4rem;
}

.ck-subtitle {
  font-family: 'EB Garamond', Georgia, serif;
  font-size: 1.25rem;
  color: var(--ck-text-muted);
  line-height: 1.35;
  margin-bottom: 1.5rem;
}
.ck-subtitle .ck-inst {
  color: var(--ck-accent);
  font-style: italic;
}

.ck-bio {
  font-size: 0.91rem;
  color: var(--ck-text-muted);
  line-height: 1.8;
  margin-bottom: 1.5rem;
}
.ck-bio a {
  color: var(--ck-link);
  text-decoration: underline;
  text-underline-offset: 2px;
}
.ck-bio a:hover { color: var(--ck-link-hover); }

.ck-address {
  font-size: 0.87rem;
  color: var(--ck-text-muted);
  line-height: 1.85;
  margin-bottom: 1.5rem;
  font-family: 'EB Garamond', Georgia, serif;
  font-size: 1rem;
}
.ck-address a { color: var(--ck-accent); text-decoration: none; }
.ck-address a:hover { text-decoration: underline; }

/* ── RIGHT ── */
.ck-right { grid-column: 2; }
@media (max-width: 720px) { .ck-right { grid-column: 1; } }

/* ── SECTIONS ── */
.ck-section { margin-bottom: 2.8rem; }

.ck-section-title {
  font-family: 'EB Garamond', Georgia, serif;
  font-size: 1.9rem;
  font-weight: 400;
  color: var(--ck-text);
  border-bottom: 1px solid var(--ck-section-rule);
  padding-bottom: 0.35rem;
  margin-bottom: 1.3rem;
}

.ck-subsection-title {
  font-family: 'EB Garamond', Georgia, serif;
  font-size: 1.1rem;
  font-style: italic;
  color: var(--ck-text-muted);
  margin: 1.5rem 0 0.9rem;
}

/* ── PAPER ── */
.ck-paper {
  margin-bottom: 1.2rem;
  padding-bottom: 1.2rem;
  border-bottom: 1px solid var(--ck-border);
  font-size: 0.9rem;
}
.ck-paper:last-child { border-bottom: none; }

.ck-paper-title {
  font-family: 'EB Garamond', Georgia, serif;
  font-size: 1.03rem;
  font-weight: 500;
  color: var(--ck-text);
  margin-bottom: 0.15rem;
}
.ck-paper-title a {
  color: var(--ck-text);
  text-decoration: underline;
  text-decoration-color: var(--ck-border);
  text-underline-offset: 2px;
  transition: color 0.2s, text-decoration-color 0.2s;
}
.ck-paper-title a:hover {
  color: var(--ck-accent);
  text-decoration-color: var(--ck-accent);
}

.ck-paper-meta {
  font-size: 0.84rem;
  color: var(--ck-text-muted);
  font-style: italic;
  margin-bottom: 0.35rem;
}

.ck-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.3rem;
  margin-bottom: 0.4rem;
}
.ck-tag {
  background: var(--ck-tag-bg);
  color: var(--ck-text-muted);
  font-size: 0.73rem;
  padding: 0.12rem 0.5rem;
  border-radius: 0.2rem;
  letter-spacing: 0.04em;
}

.ck-links {
  display: flex;
  gap: 0.6rem;
  flex-wrap: wrap;
  font-size: 0.8rem;
}
.ck-links a, .ck-abs-btn {
  color: var(--ck-accent);
  text-decoration: none;
  background: none;
  border: none;
  cursor: pointer;
  font-size: 0.8rem;
  font-family: 'Spectral', serif;
  padding: 0;
}
.ck-links a::before, .ck-abs-btn::before { content: "["; opacity: 0.55; }
.ck-links a::after,  .ck-abs-btn::after  { content: "]"; opacity: 0.55; }
.ck-links a:hover, .ck-abs-btn:hover { text-decoration: underline; }

.ck-abstract {
  display: none;
  margin-top: 0.6rem;
  font-size: 0.85rem;
  color: var(--ck-text-muted);
  line-height: 1.72;
  font-style: italic;
  border-left: 2px solid var(--ck-accent);
  padding-left: 0.8rem;
}
</style>

<div class="ck-page" id="ck-root">

  <button class="ck-toggle" onclick="ckToggle()" aria-label="Toggle colour scheme">
    <span class="ck-toggle-dot"></span>
    <span id="ck-label">light</span>
  </button>

  <div class="ck-grid">

    <!-- ══ LEFT ══ -->
    <div class="ck-left">

      <h1 class="ck-name">folan cayo<br>c. kagné</h1>

      <div class="ck-subtitle">
        PhD student<br>
        <span class="ck-inst">Paris School of Economics</span>
      </div>

      <p class="ck-bio">
        I am a doctoral researcher at the
        <a href="https://www.parisschoolofeconomics.eu/" target="_blank">Paris School of Economics</a>.
        My work sits at the intersection of experimental economics, social psychology, and political philosophy.
        I study how social exclusion, identity, and institutions shape cooperative behaviour —
        with a particular interest in carceral settings and marginalised communities.
        I also engage with Africana philosophy and decolonial thought as complementary theoretical frameworks.
        <br><br>
        <!-- Uncomment when ready:
        You can find my <a href="/assets/files/cv.pdf">curriculum vitae here</a>.
        -->
      </p>

      <div class="ck-address">
        Paris School of Economics<br>
        48 boulevard Jourdan<br>
        75014 Paris, France<br>
        <!-- email: <a href="mailto:your.email@psemail.eu">your.email@psemail.eu</a> -->
      </div>

    </div><!-- /left -->

    <!-- ══ RIGHT ══ -->
    <div class="ck-right">

      <!-- ════ WORKING PAPERS (uncomment when ready) ════

      <div class="ck-section">
        <h2 class="ck-section-title">working papers</h2>

        <div class="ck-paper">
          <div class="ck-paper-title"><a href="#">Paper Title</a></div>
          <div class="ck-paper-meta">with Coauthor — <em>revising for Journal Name</em></div>
          <div class="ck-links">
            <button class="ck-abs-btn" onclick="ckAbs('wp1')">Abstract</button>
            <a href="#">pdf</a>
          </div>
          <div class="ck-abstract" id="wp1">Abstract text here.</div>
        </div>

      </div>
      -->

      <!-- ════ WORK IN PROGRESS ════ -->
      <div class="ck-section">
        <h2 class="ck-section-title">work in progress</h2>

        <!-- econ-ish -->
        <div class="ck-subsection-title">econ-ish</div>

        <div class="ck-paper">
          <div class="ck-paper-title">Social Cooperation and Exclusion in Prisons</div>
          <div class="ck-paper-meta">Experimental economics — thesis chapter</div>
          <div class="ck-tags">
            <span class="ck-tag">social exclusion</span>
            <span class="ck-tag">cooperation</span>
            <span class="ck-tag">public goods</span>
            <span class="ck-tag">incarceration</span>
          </div>
          <div class="ck-links">
            <button class="ck-abs-btn" onclick="ckAbs('abs-prison')">Abstract</button>
          </div>
          <div class="ck-abstract" id="abs-prison">
            Over 11.5 million people are incarcerated globally, with the French prison system facing acute
            challenges such as overcrowding, poor conditions, and high recidivism. An original experiment
            was conducted in a French <em>Maison Centrale</em>, combining a public goods game, social
            inclusion priming, and qualitative interviews. The findings challenge the notion of a unified
            "criminal brotherhood" — no significant ingroup bias was observed — yet social inclusion
            priming increased cooperation toward out-group members, suggesting that minimal psychological
            interventions can foster prosociality across group boundaries.
          </div>
        </div>

        <div class="ck-paper">
          <div class="ck-paper-title">Beyond Exclusion: Social Identity and the Provision of Public Goods in Experimental Settings</div>
          <div class="ck-paper-meta">Experimental economics</div>
          <div class="ck-tags">
            <span class="ck-tag">social identity</span>
            <span class="ck-tag">public goods</span>
            <span class="ck-tag">experiment</span>
          </div>
          <div class="ck-links">
            <button class="ck-abs-btn" onclick="ckAbs('abs-beyond')">Abstract</button>
          </div>
          <div class="ck-abstract" id="abs-beyond">
            This project extends the experimental investigation of social exclusion and cooperation beyond
            carceral contexts, examining how identity salience and exclusion priming interact with
            voluntary contribution mechanisms in controlled laboratory settings.
          </div>
        </div>

        <!-- not-so-econ -->
        <div class="ck-subsection-title">not-so-econ</div>

        <div class="ck-paper">
          <div class="ck-paper-title">Philosophies et langues africaines, une introduction</div>
          <div class="ck-paper-meta">Africana philosophy — <em>en français</em></div>
          <div class="ck-tags">
            <span class="ck-tag">Africana philosophy</span>
            <span class="ck-tag">language</span>
            <span class="ck-tag">Kagamé</span>
            <span class="ck-tag">Diagne</span>
          </div>
          <div class="ck-links">
            <button class="ck-abs-btn" onclick="ckAbs('abs-langues')">Abstract</button>
          </div>
          <div class="ck-abstract" id="abs-langues">
            Cet essai explore les idées d'Alexis Kagamé sur la philosophie bantoue, mettant en avant son
            approche linguistique. Il remet en question les généralisations de Placide Tempels, soulignant
            l'importance du langage dans la pensée philosophique africaine. L'essai aborde les perspectives
            de Souleymane Bachir Diagne — encourageant à dépasser les nationalismes ontologiques pour
            embrasser la diversité philosophique — et conclut sur la proposition d'« incliner sans nécessiter ».
          </div>
        </div>

        <div class="ck-paper">
          <div class="ck-paper-title">Introduction to Africana Philosophy</div>
          <div class="ck-paper-meta">Africana philosophy — survey piece</div>
          <div class="ck-tags">
            <span class="ck-tag">Africana philosophy</span>
            <span class="ck-tag">Black existentialism</span>
            <span class="ck-tag">decolonial thought</span>
          </div>
          <div class="ck-links">
            <button class="ck-abs-btn" onclick="ckAbs('abs-afr')">Abstract</button>
          </div>
          <div class="ck-abstract" id="abs-afr">
            A survey piece situating Africana philosophy as a distinctive mode of inquiry confronting
            fundamental questions of existence, freedom, and human dignity under conditions of racialized
            oppression — drawing on Lewis Gordon, Fanon, Du Bois, and the Black radical tradition.
          </div>
        </div>

      </div><!-- /section -->

    </div><!-- /right -->

  </div><!-- /grid -->

</div><!-- /ck-page -->

<script>
  function ckAbs(id) {
    var el = document.getElementById(id);
    if (!el) return;
    el.style.display = el.style.display === 'block' ? 'none' : 'block';
  }

  function ckToggle() {
    var root = document.getElementById('ck-root');
    var isDark = root.getAttribute('data-ck-theme') === 'dark';
    root.setAttribute('data-ck-theme', isDark ? '' : 'dark');
    document.getElementById('ck-label').textContent = isDark ? 'light' : 'dark';
  }

  // Match OS preference on load
  if (window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches) {
    document.getElementById('ck-root').setAttribute('data-ck-theme', 'dark');
    document.getElementById('ck-label').textContent = 'dark';
  }
</script>
