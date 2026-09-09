# ladinomishel26-debug.github.io
Newspaper
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>The Minds-On Times</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,500;0,600;0,700;1,400&family=Space+Mono:wght@400;700&display=swap');

  :root{
    --paper:#EFE6D3;
    --paper-dark:#E6D9BE;
    --ink:#211D17;
    --ink-soft:#4A4335;
    --green:#3F5D48;
    --mustard:#C68A2E;
    --brick:#8C3B2E;
    --rule:#C9B98F;
  }

  *{box-sizing:border-box;}

  body{
    margin:0;
    background:#D9CDA9;
    font-family:'Lora', serif;
    color:var(--ink);
    display:flex;
    justify-content:center;
    padding:24px 12px;
  }

  .page{
    background:var(--paper);
    width:100%;
    max-width:1100px;
    padding:36px 44px 28px;
    box-shadow:0 4px 30px rgba(0,0,0,0.25);
    background-image:
      radial-gradient(circle at 12% 8%, rgba(0,0,0,0.02) 0%, transparent 40%),
      radial-gradient(circle at 90% 90%, rgba(0,0,0,0.02) 0%, transparent 45%);
  }

  /* MASTHEAD */
  .dateline{
    display:flex;
    justify-content:space-between;
    font-family:'Space Mono', monospace;
    font-size:11px;
    letter-spacing:0.03em;
    color:var(--ink-soft);
    border-bottom:1px solid var(--ink);
    padding-bottom:6px;
  }

  .masthead{
    text-align:center;
    padding:14px 0 10px;
    border-bottom:4px double var(--ink);
  }

  .masthead h1{
    margin:0;
    font-size:66px;
    font-weight:700;
    letter-spacing:0.01em;
    line-height:1;
  }

  .masthead .tagline{
    margin-top:8px;
    font-style:italic;
    font-size:15px;
    color:var(--ink-soft);
  }

  .kicker-row{
    display:flex;
    justify-content:space-between;
    font-family:'Space Mono', monospace;
    font-size:11px;
    color:var(--ink-soft);
    padding:6px 0;
    border-bottom:1px solid var(--ink);
  }

  /* HERO / LEAD */
  .hero{
    display:grid;
    grid-template-columns:1.6fr 1fr;
    gap:30px;
    padding:24px 0 20px;
    border-bottom:2px solid var(--ink);
  }

  .hero h2{
    font-size:44px;
    line-height:1.05;
    margin:0 0 6px;
    font-weight:700;
  }

  .hero .quote-mark{
    color:var(--brick);
  }

  .byline{
    font-family:'Space Mono', monospace;
    font-size:11px;
    color:var(--ink-soft);
    margin-bottom:14px;
    text-transform:uppercase;
    letter-spacing:0.06em;
  }

  .hero p{
    font-size:16px;
    line-height:1.55;
    margin:0 0 12px;
    max-width:62ch;
  }

  .hero .dropcap{
    float:left;
    font-size:64px;
    line-height:0.8;
    padding:6px 8px 0 0;
    font-weight:700;
    color:var(--brick);
  }

  .pull-panel{
    background:var(--paper-dark);
    border-left:4px solid var(--green);
    padding:18px 20px;
  }

  .pull-panel h3{
    margin:0 0 10px;
    font-size:15px;
    text-transform:uppercase;
    letter-spacing:0.05em;
    color:var(--green);
    font-family:'Space Mono', monospace;
  }

  .pull-panel blockquote{
    margin:0 0 14px;
    font-style:italic;
    font-size:17px;
    line-height:1.4;
    border-bottom:1px solid var(--rule);
    padding-bottom:14px;
  }

  .pull-panel ol{
    margin:0;
    padding-left:20px;
    font-size:14.5px;
    line-height:1.5;
  }

  .pull-panel li{margin-bottom:8px;}

  /* THREE COLUMN BODY */
  .body-grid{
    display:grid;
    grid-template-columns:1fr 1fr 1fr;
    gap:26px;
    padding:22px 0;
    border-bottom:2px solid var(--ink);
  }

  .body-grid h4{
    font-size:19px;
    margin:0 0 10px;
    border-bottom:2px solid var(--mustard);
    display:inline-block;
    padding-bottom:3px;
  }

  .body-grid p{
    font-size:14px;
    line-height:1.55;
    margin:0 0 10px;
  }

  .checklist{
    list-style:none;
    margin:0;
    padding:0;
    font-size:14px;
    line-height:1.5;
  }
  .checklist li{
    padding-left:22px;
    position:relative;
    margin-bottom:9px;
  }
  .checklist li::before{
    content:"✓";
    position:absolute;
    left:0;
    color:var(--green);
    font-weight:700;
  }

  /* COMPARISON */
  .comparison{
    padding:22px 0;
    border-bottom:2px solid var(--ink);
  }

  .comparison h3{
    text-align:center;
    font-size:24px;
    margin:0 0 4px;
  }
  .comparison .sub{
    text-align:center;
    font-family:'Space Mono', monospace;
    font-size:11px;
    color:var(--ink-soft);
    margin-bottom:18px;
  }

  .vs-grid{
    display:grid;
    grid-template-columns:1fr 60px 1fr;
    gap:0;
    align-items:stretch;
  }

  .vs-col{
    padding:16px 20px;
  }
  .vs-col.fun{
    border:2px solid var(--brick);
    background:rgba(140,59,46,0.05);
  }
  .vs-col.deep{
    border:2px solid var(--green);
    background:rgba(63,93,72,0.06);
  }

  .vs-col h5{
    margin:0 0 10px;
    font-size:16px;
    text-transform:uppercase;
    letter-spacing:0.04em;
    font-family:'Space Mono', monospace;
  }
  .vs-col.fun h5{color:var(--brick);}
  .vs-col.deep h5{color:var(--green);}

  .vs-col ul{
    margin:0;
    padding-left:18px;
    font-size:13.5px;
    line-height:1.5;
  }
  .vs-col li{margin-bottom:7px;}

  .vs-divider{
    display:flex;
    align-items:center;
    justify-content:center;
    font-family:'Space Mono', monospace;
    font-weight:700;
    font-size:15px;
    color:var(--ink-soft);
  }

  /* ADS */
  .ads{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:24px;
    padding-top:20px;
  }

  .ad{
    border:3px solid var(--ink);
    padding:16px 18px;
    background:var(--paper-dark);
    position:relative;
  }

  .ad .ad-label{
    position:absolute;
    top:-11px;
    left:14px;
    background:var(--paper);
    padding:0 8px;
    font-family:'Space Mono', monospace;
    font-size:10px;
    letter-spacing:0.08em;
    color:var(--ink-soft);
  }

  .ad h4{
    margin:6px 0 6px;
    font-size:19px;
  }

  .ad p{
    font-size:13.5px;
    line-height:1.5;
    margin:0 0 8px;
  }

  .ad .cta{
    display:inline-block;
    font-family:'Space Mono', monospace;
    font-size:11.5px;
    border:1.5px solid var(--ink);
    padding:5px 10px;
    letter-spacing:0.03em;
  }

  .footer-strip{
    margin-top:22px;
    padding-top:10px;
    border-top:1px solid var(--ink);
    text-align:center;
    font-family:'Space Mono', monospace;
    font-size:10.5px;
    color:var(--ink-soft);
  }

  @media (max-width:820px){
    .hero{grid-template-columns:1fr;}
    .body-grid{grid-template-columns:1fr;}
    .vs-grid{grid-template-columns:1fr;}
    .vs-divider{padding:8px 0;}
    .ads{grid-template-columns:1fr;}
    .masthead h1{font-size:42px;}
    .hero h2{font-size:30px;}
  }
</style>
</head>
<body>
<div class="page">

  <div class="dateline">
    <span>EARLY CHILDHOOD EDITION</span>
    <span>ESTABLISHED BY THE STUDY OF JOHN DEWEY</span>
  </div>

  <div class="masthead">
    <h1>The Minds-On Times</h1>
    <div class="tagline">"Hands busy is not the same as minds engaged." — reporting on the educational philosophy of John Dewey</div>
  </div>

  <div class="kicker-row">
    <span>VOL. I · NO. 1</span>
    <span>SOURCE: THEORIES OF CHILDHOOD, CH. 1 — JOHN DEWEY, P. 29</span>
    <span>PRICE: YOUR FULL ATTENTION</span>
  </div>

  <div class="hero">
    <div class="hero-main">
      <div class="byline">Front Page Feature</div>
      <h2><span class="quote-mark">"</span>It's Fun<span class="quote-mark">"</span> Is Not Enough</h2>
      <p><span class="dropcap">D</span>ewey believed that when children are engaged in something that interests them and connects to their own experience, learning naturally becomes enjoyable. But he issued a sharp warning to teachers: enjoyment on its own does not prove that learning is happening. A classroom can be full of laughter and still teach nothing at all.</p>
      <p>According to Dewey, teachers should never justify an activity simply because "the children will enjoy this." Instead, every activity must be tested against a deeper question: does it actually grow a child's understanding, skill, and ability to make sense of the world?</p>
      <p>It is not enough, Dewey argued, for an activity to be "hands-on." It must also be "minds-on" — and that only happens when teachers invest real thought into organizing the experience and documenting what children discover along the way.</p>
    </div>

    <div class="pull-panel">
      <h3>The Big Idea</h3>
      <blockquote>Fun is a byproduct of real learning — not a substitute for it.</blockquote>
      <h3 style="margin-top:14px;">Questions Every Teacher Should Ask</h3>
      <ol>
        <li>How does this expand on what children already know?</li>
        <li>How will this activity help this child grow?</li>
        <li>What skills are being developed?</li>
        <li>How does this add to children's understanding of their world?</li>
        <li>How does this prepare children to live more fully?</li>
      </ol>
    </div>
  </div>

  <div class="body-grid">
    <div>
      <h4>Education vs. Mis-Education</h4>
      <p>Dewey drew a firm line between real learning and what he called "mis-educative" experiences — activities that feel busy or exciting but lack real purpose or structure.</p>
      <p>He criticized old-fashioned rote memorization just as much as he criticized the opposite extreme: turning children loose with no guidance, theme, or continuity at all.</p>
    </div>
    <div>
      <h4>What Makes It Educational</h4>
      <p>Dewey held that an experience only counts as truly educational when it meets a clear set of standards, checked off below:</p>
      <ul class="checklist">
        <li>Grows out of children's own interests and knowledge</li>
        <li>Supports their ongoing development</li>
        <li>Builds new, usable skills</li>
        <li>Deepens understanding of the world</li>
        <li>Prepares children to live more fully</li>
      </ul>
    </div>
    <div>
      <h4>Why Documentation Matters</h4>
      <p>A teacher's job doesn't end when the activity does. Dewey emphasized that observing, recording, and reflecting on what children say and discover is what turns a fun moment into a foundation for future learning.</p>
      <p>Without that documentation, even a lively activity risks becoming a one-off event that leads nowhere.</p>
    </div>
  </div>

  <div class="comparison">
    <h3>Two Ice Cream Parties, Two Very Different Outcomes</h3>
    <div class="sub">A CASE STUDY IN "HANDS-ON" VS. "MINDS-ON"</div>
    <div class="vs-grid">
      <div class="vs-col fun">
        <h5>Party One: Fun Without Depth</h5>
        <ul>
          <li>Children pick toppings and enjoy a sundae celebration</li>
          <li>No connection to prior knowledge or curiosity</li>
          <li>Documentation limited to a flawed "favorite flavor" chart</li>
          <li>Activity ends with no follow-up questions or wonder</li>
        </ul>
      </div>
      <div class="vs-divider">VS</div>
      <div class="vs-col deep">
        <h5>Party Two: Fun With Purpose</h5>
        <ul>
          <li>Starts from real curiosity: none had tasted peach ice cream</li>
          <li>Children's ideas are asked for, recorded, and built upon</li>
          <li>Family interviews, a factory visit, and hands-on ice-cream making</li>
          <li>Sparks a brand-new investigation: pre-electricity refrigeration</li>
        </ul>
      </div>
    </div>
  </div>

  <div class="ads">
    <div class="ad">
      <div class="ad-label">ADVERTISEMENT</div>
      <h4>The Minds-On Planner™</h4>
      <p>A teacher's planning notebook built around Dewey's five questions. Every page prompts you to document what children already know, what they're curious about, and where the inquiry might grow next — so no activity ends where it started.</p>
      <span class="cta">Plan with purpose →</span>
    </div>
    <div class="ad">
      <div class="ad-label">ADVERTISEMENT</div>
      <h4>Curiosity Cart Field Trips</h4>
      <p>Turn any classroom topic into a real-world investigation. From ice cream factories to community gardens, our guided visits help children connect what they're learning in class to the wider world — exactly the kind of experience Dewey called truly educational.</p>
      <span class="cta">Book an expedition →</span>
    </div>
  </div>

  <div class="footer-strip">
    ADAPTED FROM CAROL GARHART MOONEY, <em>THEORIES OF CHILDHOOD</em> (REDLEAF PRESS, 2013), P. 29–31 · A CLASSROOM GAZETTE PUBLICATION
  </div>

</div>
</body>
</html>
