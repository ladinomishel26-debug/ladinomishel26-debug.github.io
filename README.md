# ladinomishel26-debug.github.io
<>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>The Blocks &amp; Books Bulletin</title>
<style>
  :root{
    --paper:#E9E1CB;
    --paper-dark:#DDD3B6;
    --ink:#221D16;
    --rule:#8B7E63;
    --dewey:#7C3626;
    --dewey-tint:#F1E2D8;
    --monte:#33544A;
    --monte-tint:#DFE6DE;
  }
  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;}
  body{
    background:#C9BFA4;
    font-family:Georgia, "Iowan Old Style", "Palatino Linotype", serif;
    color:var(--ink);
    display:flex;
    justify-content:center;
    padding:18px;
  }
  .page{
    width:100%;
    max-width:1180px;
    background:
      radial-gradient(ellipse at top left, rgba(255,255,255,0.25), transparent 60%),
      var(--paper);
    border:1px solid #b9ac8b;
    box-shadow:0 10px 30px rgba(0,0,0,0.25);
    padding:34px 42px 26px;
  }

  .masthead{
    text-align:center;
    border-bottom:4px double var(--ink);
    padding-bottom:10px;
    margin-bottom:8px;
  }
  .kicker{
    display:flex;
    justify-content:space-between;
    font-size:11px;
    letter-spacing:0.08em;
    color:var(--ink);
    border-bottom:1px solid var(--rule);
    padding-bottom:6px;
    margin-bottom:10px;
  }
  .title{
    font-family:"Times New Roman", Times, "Palatino Linotype", serif;
    font-weight:700;
    font-size:64px;
    line-height:0.95;
    letter-spacing:0.5px;
    margin:2px 0 6px;
  }
  .title .amp{
    font-style:italic;
    font-weight:400;
    padding:0 6px;
  }
  .subhead{
    font-size:14px;
    font-style:italic;
    color:#4a4234;
  }

  .duel{
    display:grid;
    grid-template-columns:1fr 3px 1fr;
    gap:0 26px;
    margin-top:22px;
  }
  .divider{
    background:var(--ink);
    opacity:0.75;
  }
  .col{padding-top:2px;}

  .byline-tag{
    font-size:12px;
    font-style:italic;
    letter-spacing:0.03em;
    margin-bottom:4px;
  }
  .dewey .byline-tag{color:var(--dewey);}
  .monte .byline-tag{color:var(--monte);}

  h2.headline{
    font-family:Georgia, serif;
    font-size:30px;
    line-height:1.08;
    margin:0 0 4px;
  }
  .dewey h2.headline{color:var(--dewey);}
  .monte h2.headline{color:var(--monte);}

  .dek{
    font-size:14.5px;
    font-style:italic;
    color:#463d30;
    margin-bottom:10px;
    line-height:1.35;
  }

  .body-text{
    columns:2;
    column-gap:20px;
    font-size:13.3px;
    line-height:1.5;
    text-align:justify;
  }
  .body-text p{margin:0 0 10px;}
  .body-text p:first-of-type::first-letter{
    float:left;
    font-size:42px;
    line-height:0.8;
    padding:4px 6px 0 0;
    font-weight:700;
  }
  .dewey .body-text p:first-of-type::first-letter{color:var(--dewey);}
  .monte .body-text p:first-of-type::first-letter{color:var(--monte);}

  .pullquote{
    break-inside:avoid;
    border-left:3px solid;
    margin:6px 0 10px;
    padding:2px 0 2px 12px;
    font-size:14px;
    font-style:italic;
    line-height:1.35;
  }
  .dewey .pullquote{border-color:var(--dewey); color:var(--dewey);}
  .monte .pullquote{border-color:var(--monte); color:var(--monte);}

  .takeaway{
    margin-top:8px;
    padding-top:8px;
    border-top:1px solid var(--rule);
    font-size:12.5px;
  }
  .takeaway strong{display:block; font-size:11px; letter-spacing:0.05em; margin-bottom:3px;}
  .dewey .takeaway strong{color:var(--dewey);}
  .monte .takeaway strong{color:var(--monte);}

  .ads{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:22px;
    margin-top:22px;
    border-top:4px double var(--ink);
    padding-top:16px;
  }
  .ad{
    border:2px solid var(--ink);
    padding:14px 16px;
    display:flex;
    gap:14px;
    align-items:center;
    background:rgba(255,255,255,0.35);
    position:relative;
  }
  .ad-label{
    position:absolute;
    top:-10px;
    left:14px;
    background:var(--paper);
    padding:0 8px;
    font-size:10px;
    letter-spacing:0.1em;
    color:var(--ink);
    font-style:normal;
  }
  .ad-icon{flex:0 0 64px;}
  .ad-copy h3{
    margin:0 0 4px;
    font-size:16px;
    line-height:1.15;
  }
  .ad-copy p{
    margin:0;
    font-size:11.5px;
    line-height:1.35;
    font-style:italic;
  }
  .ad.dewey-ad h3{color:var(--dewey);}
  .ad.monte-ad h3{color:var(--monte);}

  .footer{
    margin-top:18px;
    padding-top:8px;
    border-top:1px solid var(--rule);
    display:flex;
    justify-content:space-between;
    align-items:baseline;
    font-size:11.5px;
    color:#4a4234;
  }
  .staff{
    font-style:italic;
  }
  .staff b{
    font-style:normal;
  }

  @media (max-width:760px){
    .page{padding:20px;}
    .title{font-size:38px;}
    .duel{grid-template-columns:1fr; gap:22px;}
    .divider{display:none;}
    .body-text{columns:1;}
    .ads{grid-template-columns:1fr;}
  }
</style>
</head>
<body>
<div class="page">

  <div class="masthead">
    <div class="kicker">
      <span>EARLY CHILDHOOD EDUCATION EDITION</span>
      <span>ONE COPY, TWO GREAT THINKERS</span>
      <span>PRICE: YOUR FULL ATTENTION</span>
    </div>
    <div class="title">THE BLOCKS <span class="amp">&amp;</span> BOOKS BULLETIN</div>
    <div class="subhead">Reporting on how children really learn straight from the classroom desk of Dewey &amp; Montessori</div>
  </div>

  <div class="duel">

    <div class="col dewey">
      <div class="byline-tag">FEATURE &middot; From the Desk of John Dewey</div>
      <h2 class="headline">Beyond the Sundae Bar: Why "Fun" Isn't Enough</h2>
      <div class="dek">A classroom ice-cream party looked joyful but did it teach anything? Dewey says enjoyment is only step one.</div>
      <div class="body-text">
        <p>John Dewey argued that learning should absolutely be enjoyable, but he warned teachers not to stop there. An experience can be exciting and still teach nothing, if it isn't connected to what children already know or curious about.</p>
        <div class="pullquote">"The children really seemed to enjoy it" is not the same as "the children really learned something."</div>
        <p>Take the make your own sundae day one educator described: children picked toppings, taped paper cones to a "Favorite Ice Cream" chart, and had a wonderful time. But the activity never asked what the children already knew about ice cream, never built new skills, and the final chart didn't even leave room for real answers one child's true favorite, Cherry Garcia, simply didn't fit the categories.</p>
        <p>By ending on a tidy "my favorite is..." chart, the teacher closed the door on curiosity instead of opening it. Dewey's lesson: good planning starts with the child's experience and pushes it somewhere new, rather than just delivering a good time.</p>
      </div>
      <div class="takeaway">
        <strong>THE TAKEAWAY</strong>
        Plan for interest AND growth. Ask what children already know, what they wonder about next, and how the activity builds a real skill, not just a smile.
      </div>
    </div>

    <div class="divider"></div>

    <div class="col monte">
      <div class="byline-tag">FEATURE &middot; From the Desk of Maria Montessori</div>
      <h2 class="headline">Let Them Do It Themselves: Montessori on Growing Up Capable</h2>
      <div class="dek">Every task an adult does for a child is a lesson the child doesn't get to learn. Montessori says: step back.</div>
      <div class="body-text">
        <p>Maria Montessori believed children have a deep drive to care for themselves and their surroundings, and that adults, often without meaning to, get in the way. She cautioned that grown-ups "serve" children far too much, doing things for them that they could be doing for themselves.</p>
        <div class="pullquote">Children who are never allowed to do something for themselves never learn how to do it.</div>
        <p>It is almost always faster for an adult to just pour the juice, button the coat, or sweep up the spill. But Montessori insisted that real growth requires handing that job back to the child, even when it's slower and messier.</p>
        <p>She also observed that children learn through repetition, doing the same task again and again until it becomes truly their own. Her advice to teachers: prepare a rich environment, offer real materials, then step back and give children the time and space to practice uninterrupted.</p>
      </div>
      <div class="takeaway">
        <strong>THE TAKEAWAY</strong>
        Hand responsibility back to children. Give them real jobs, real tools, and long uninterrupted blocks of time to practice at their own pace.
      </div>
    </div>

  </div>

  <div class="ads">
    <div class="ad dewey-ad">
      <div class="ad-label">ADVERTISEMENT</div>
      <div class="ad-icon">
        <svg width="60" height="60" viewBox="0 0 60 60" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M18 26 L42 26 L34 54 L26 54 Z" fill="#7C3626" opacity="0.85"/>
          <circle cx="30" cy="20" r="12" fill="#7C3626"/>
          <circle cx="24" cy="15" r="2" fill="#E9E1CB"/>
          <circle cx="33" cy="12" r="2" fill="#E9E1CB"/>
          <circle cx="36" cy="20" r="2" fill="#E9E1CB"/>
        </svg>
      </div>
      <div class="ad-copy">
        <h3>THE "WHAT DO YOU WONDER?" SUNDAE CART</h3>
        <p>Not just toppings question cards included! Ask what children already know before the first scoop. Turns snack time into a real Dewey approved investigation. Curiosity not included, but strongly encouraged.</p>
      </div>
    </div>
    <div class="ad monte-ad">
      <div class="ad-label">ADVERTISEMENT</div>
      <div class="ad-icon">
        <svg width="60" height="60" viewBox="0 0 60 60" fill="none" xmlns="http://www.w3.org/2000/svg">
          <rect x="14" y="30" width="10" height="22" rx="1" fill="#33544A"/>
          <rect x="26" y="20" width="10" height="32" rx="1" fill="#33544A" opacity="0.85"/>
          <rect x="38" y="12" width="10" height="40" rx="1" fill="#33544A" opacity="0.7"/>
        </svg>
      </div>
      <div class="ad-copy">
        <h3>LITTLE HANDS, REAL TOOLS</h3>
        <p>Child-sized brooms, pitchers, and folding cloths, sized for small hands and big independence. No plastic toy versions here, just real jobs, done by real children, over and over until they've got it.</p>
      </div>
    </div>
  </div>

  <div class="footer">
    <div class="staff"><b>Reporting &amp; Editorial Team:</b> Add your group members' full names here</div>
    <div>Vol. I &middot; No. 1 &middot; Sources: Dewey, "'It's Fun' Is Not Enough" &amp; Montessori, "Competence and Responsibility"</div>
  </div>

</div>
</body>
</html>
