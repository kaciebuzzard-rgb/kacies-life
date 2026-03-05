---
layout: default
title: Home
---

/* =========================
   HERO (MATCHES YOUR HTML)
========================= */
.hero{
  position:relative;
  padding:112px 0 72px;
  min-height:78vh;
  display:flex;
  align-items:center;

  /* CHANGE THIS FILE NAME to match your real hero image */
  background:
    url('/assets/img/hero.jpg') center/cover no-repeat;
}

/* Your markup includes a real overlay div */
.hero-overlay{
  position:absolute;
  inset:0;
  /* dark overlay for readability */
  background:rgba(25,20,18,.45);
  pointer-events:none;
}

/* Ensure hero content sits above overlay */
.hero-inner{
  position:relative;
  z-index:1;
  max-width:760px;
}

.hero h1{
  color:#fff;
  font-size:clamp(34px, 5vw, 56px);
  letter-spacing:-.6px;
  margin:0 0 14px;
}

.hero-sub{
  color:rgba(255,255,255,.92);
  font-size:clamp(16px, 2vw, 20px);
  margin:0 0 22px;
  opacity:1;
}

/* Buttons row */
.hero-buttons{
  display:flex;
  gap:12px;
  flex-wrap:wrap;
  margin-top:10px;
}

/* Make ghost readable on dark hero */
.btn-ghost{
  background:rgba(255,255,255,.14);
  color:#fff;
  border:1px solid rgba(255,255,255,.22);
  box-shadow:none;
}
.btn-ghost:hover{
  background:rgba(255,255,255,.20);
}

/* =========================
   OUTLINE BUTTON (you used .btn-outline)
========================= */
.btn-outline{
  background:transparent;
  color:#1e1b18;
  border:1px solid rgba(30,27,24,.22);
  box-shadow:none;
}
.btn-outline:hover{
  background:rgba(197,90,58,.10);
  border-color:rgba(197,90,58,.35);
}

<section id="about">
  <div class="wrap about-grid">
    <div class="about-text">
      <h2>About Kacie</h2>

      <p>
        Kacie Wielgus (Buzzard) is a speaker, writer, and strategist working at the intersection of
        disability advocacy, caregiving systems, and inclusive communications.
      </p>

      <p>
        Drawing on lived experience as a parent navigating complex medical and disability systems,
        her work helps organizations move beyond awareness toward structural change.
      </p>

      <p>
        Her writing explores caregiving, invisible labor, disability identity, and the systems families
        must navigate. Her keynotes challenge audiences to rethink how policy, communication, and leadership
        shape the lives of disabled people and their families.
      </p>

      <a class="btn btn-outline" href="/about">Read Full Bio</a>
    </div>

    <div class="about-image">
      <img
        src="{{ '/assets/img/kacie-speaking.jpg' | relative_url }}"
        alt="Kacie Buzzard speaking about disability advocacy and caregiving systems">
    </div>
  </div>
</section>
