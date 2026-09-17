---
layout: page
permalink: /research/
title: "Research"
eyebrow: "What I work on"
lede: "I primarily study core-collapse supernovae across the full span of their evolution: from shock-cooling emission in the first hours to days, to cold dust condensing in the ejecta thousands of days later, and I help build the systems that make catching those moments possible."
description: "Research projects: JWST/MIRI dust formation in core-collapse supernovae, early shock-cooling observations of young transients, the extreme nuclear transient AT 2021lwx, electromagnetic counterparts to gravitational-wave events, REFITT, and the JWST survey of Cassiopeia A."
---

<!--
  ══════════════════════════════════════════════════════════════
  HOW TO ADD A PROJECT
  ──────────────────────────────────────────────────────────────
  With a figure:  copy a <section class="project"> block. Figures always
  render on the right; there is no side to choose.
  Without a figure: copy the "project project--noimage" block; its text
  column keeps the same width as every other section.
  The id="..." is what the home-page cards link to.
  ══════════════════════════════════════════════════════════════
-->

<!-- ─────────────────────── 1. JWST DUST ────────────────────── -->
<section class="project" id="jwst-dust">
  <figure class="project__figure project__figure--plate">
    <img src="{{ '/images/dust_timeline_mdot_new_copy.png' | relative_url }}"
         alt="Dust mass against phase for eleven Type IIP supernovae, coloured by progenitor mass-loss rate, with literature comparison objects"
         loading="lazy" decoding="async">
    <figcaption>
Dust mass as a function of phase for our 11 SNe (large colored symbols) and comparison objects from the literature (small symbols). Symbol color for only the 11 SNe encodes the progenitor mass-loss rate, as shown in the color-bar, with gold rings marking SNe with detected early flash-ionization features. The mass-loss rates shown in this figure are heterogeneous literature estimates derived under different assumptions and should be viewed as qualitative indicators of relative CSM strength (<a href="https://arxiv.org/abs/2608.16979">Subrayan et&nbsp;al. 2026</a>).
    </figcaption>
  </figure>
  <div class="project__body">
    <span class="eyebrow">JWST &middot; MIRI &middot; Dust</span>
    <h2 class="project__title">Dust factories in ordinary core-collapse supernovae</h2>

    <p>
      Core-collapse supernovae are among the leading candidates for the dust that fills
      young galaxies, but almost everything we know observationally comes from a handful
      of famous objects, SN&nbsp;1987A, Cassiopeia&nbsp;A. The obvious question is
      whether <em>normal</em> supernovae behave the same way.
    </p>

    <p>
      With JWST/MIRI I am assembling the first uniform mid-infrared sample built to answer
      that: eleven nearby Type&nbsp;IIP supernovae, among them SN&nbsp;2017eaw,
      SN&nbsp;2020jfo, SN&nbsp;2021gmj, SN&nbsp;2021yja, SN&nbsp;2022acko, SN&nbsp;2023ixf
      and SN&nbsp;2024ggi; observed between roughly 400 and 2300 days after
      explosion. Modelling their warm and cold dust components on a common footing lets us
      trace a dust-formation timeline rather than a single snapshot, and separate newly
      condensed grains from infrared echoes and circumstellar-interaction heating.
    </p>

    <p class="mt-1">
      I lead the Keck and Gemini spectroscopic campaigns that support this work, searching
      for late-time signatures of circumstellar interaction and dust formation in the same
      objects, and I am a co-investigator on JWST programs watching dust condense in real
      time in two very nearby core-collapse supernovae.
    </p>

    <div class="links">
       <a href="https://arxiv.org/abs/2608.16979">arXiv:2608.16979</a>
      <a href="https://ui.adsabs.harvard.edu/abs/2025ApJ...993..213P/abstract">Companion paper: SN 2017eaw</a>
      <a href="{{ '/publications/' | relative_url }}">Publications</a>
    </div>
  </div>
</section>

<!-- ──────────────────── 2. YOUNG TRANSIENTS ────────────────── -->
<section class="project" id="young-transients">
  <figure class="project__figure">
    <img src="{{ '/images/SN2024uwq_light_curve.png' | relative_url }}"
         alt="Early multi-band light curve of the Type IIb SN 2024uwq with shock-cooling models"
         loading="lazy" decoding="async">
    <figcaption>
      Shock breakout and cooling-envelope emission carry information about the radius and
      envelope structure of a stripped-envelope progenitor, but only for the first
      few days (<a href="https://iopscience.iop.org/article/10.3847/2041-8213/adfe52">Subrayan et&nbsp;al. 2025</a>).
    </figcaption>
  </figure>

  <div class="project__body">
    <span class="eyebrow">Progenitors &middot; Early time</span>
    <h2 class="project__title">The earliest moments after a SN explosion</h2>

    <p>
      When a massive star explodes, the shock breaking out of its surface produces a brief
      cooling phase whose brightness and colour evolution depend directly on how big the
      star was. Catch it, and you measure the progenitor. Miss it by two days, and the
      information is gone.
    </p>

    <p>
      I led the discovery and analysis of early shock-cooling emission in the
      Type&nbsp;IIb <strong>SN&nbsp;2024uwq</strong>, using rapid multi-band photometry
      and spectroscopy to constrain the radius and envelope mass of a partially stripped
      progenitor. Applied to a statistical sample, which the Rubin Observatory era will
      finally make possible, the same approach can tell us what fraction of
      stripped-envelope supernovae hold on to an extended envelope at all, and how that
      connects to their mass-loss history.
    </p>

    <p>
      To get ahead of that, I am PI of Bok/90Prime programs at Steward that pilot
      early-transient discovery with ZTF, and lay groundwork for UV transient science with
      ULTRASAT.
    </p>

    <div class="links">
      <a href="https://ui.adsabs.harvard.edu/abs/2025ApJ...990L..68S/abstract">ADS</a>
      <a href="https://arxiv.org/abs/2505.02908">arXiv:2505.02908</a>
      <a href="https://iopscience.iop.org/article/10.3847/2041-8213/adfe52">ApJL</a>
    </div>
  </div>
</section>

<!-- ───────────────────────── 3. AT 2021lwx ─────────────────── -->
<section class="project" id="at2021lwx">
  <figure class="project__figure project__figure--plate">
    <!-- Animated version of the light curve. The .gif of the same animation is
         in images/ if you ever want a plain <img> instead; the video is ~10x
         lighter. images/Scary_Barbie.png is the original still. -->
    <video src="{{ '/images/AT2021lwx_lightcurve.mp4' | relative_url }}"
           poster="{{ '/images/AT2021lwx_lightcurve.jpg' | relative_url }}"
           autoplay loop muted playsinline preload="metadata"
           aria-label="Animated rest-frame absolute magnitude light curve of AT 2021lwx compared with other luminous transients"></video>
    <figcaption>
      Rest-frame ZTF-<em>r</em> absolute light curve of AT&nbsp;2021lwx compared with other
      luminous transients (<a href="https://iopscience.iop.org/article/10.3847/2041-8213/accf1a">Subrayan et&nbsp;al. 2023</a>).
    </figcaption>
  </figure>

  <div class="project__body">
    <span class="eyebrow">Extreme nuclear transients</span>
    <h2 class="project__title">AT&nbsp;2021lwx, &ldquo;Scary Barbie&rdquo;</h2>

    <p>
      AT&nbsp;2021lwx is the most energetic accretion event yet observed. At a
      spectroscopically measured redshift of <em>z</em>&nbsp;=&nbsp;0.995 it reached a peak
      pseudo-bolometric luminosity of log(<em>L</em>/[erg&nbsp;s<sup>&minus;1</sup>])&nbsp;=&nbsp;45.7
      and stayed bright across more than 1000 observer-frame days. It is too smooth for
      AGN flaring, and too luminous for any supernova we have seen or modelled.
    </p>

    <p>
      The optical spectra show strong, narrow-cored Balmer emission and semi-forbidden
      Si&nbsp;III], C&nbsp;III] and C&nbsp;II] lines, with none of the [O&nbsp;II] or
      [O&nbsp;III] that normally betrays an active nucleus. We concluded that this is most
      likely an extreme tidal disruption event: modelling the ZTF photometry with MOSFiT
      points to a &asymp;14&nbsp;M<sub>&#9737;</sub> star disrupted by a
      &sim;10<sup>8</sup>&nbsp;M<sub>&#9737;</sub> black hole. Remarkably, no host galaxy
      has been detected.
    </p>

    <p>
      I am now PI of an HST program and a JWST Cycle&nbsp;5 program (GO-11424) designed to
      find that host and test black-hole&ndash;host scaling relations for extreme nuclear
      transients, with a late-time analysis paper in preparation.
    </p>

    <div class="links">
      <a href="https://ui.adsabs.harvard.edu/abs/2023ApJ...948L..19S/abstract">ADS</a>
      <a href="https://arxiv.org/abs/2302.10932">arXiv:2302.10932</a>
      <a href="https://iopscience.iop.org/article/10.3847/2041-8213/accf1a">ApJL</a>
      <a href="{{ '/files/AT2021lwx_Scary_Barbie_data.tar.gz' | relative_url }}">Data</a>
      <a href="https://the1a.org/segments/scientific-method-when-a-supermassive-black-hole-devours-a-star/">NPR 1A</a>
    </div>
  </div>
</section>

<!-- ─────────────── 4. GRAVITATIONAL-WAVE FOLLOW-UP ────────── -->
<section class="project" id="gravitational-waves">
  <div class="project__aside">
    <figure class="project__badge">
      <a href="http://sand.as.arizona.edu/saguaro_tom/">
        <img src="{{ '/images/SAGUARO_badge.png' | relative_url }}"
             alt="SAGUARO project logo: a telescope trained on the sky above a saguaro cactus"
             loading="lazy" decoding="async">
      </a>
      <figcaption>
        <a href="http://sand.as.arizona.edu/saguaro_tom/">Searches After Gravitational waves
        Using ARizona Observatories</a>
      </figcaption>
    </figure>

    <figure class="project__badge">
      <a href="https://datatrove-test.as.arizona.edu/">
        <img src="{{ '/images/TROVE_badge.jpg' | relative_url }}"
             alt="TROVE project logo: a treasure chest and a saguaro cactus under a night sky with a transient"
             loading="lazy" decoding="async">
      </a>
      <figcaption>
        <a href="https://datatrove-test.as.arizona.edu/">Tool for Rapid Object Vetting and
        Examination</a>
      </figcaption>
    </figure>

    <figure class="project__figure project__figure--plate">
      <img src="{{ '/images/SN2025ulz_shock_cooling.png' | relative_url }}"
         alt="Shock-cooling model fits to the griI and HST F336W light curves of SN 2025ulz for polytropic indices n = 3/2 and n = 3"
         loading="lazy" decoding="async">
    <figcaption>
      Fits of the <em>griI</em> and HST F336W (comparable to Swift/UVOT <em>U</em>-band) light
      curves of SN&nbsp;2025ulz with a shock-cooling model (N.&nbsp;Sapir &amp; E.&nbsp;Waxman
      2017), assuming two polytropic indices: <em>n</em>&nbsp;=&nbsp;3/2 (left) and
      <em>n</em>&nbsp;=&nbsp;3 (right). The best-fit explosion date, with uncertainties, and the
      detection date of S250818k are shown as grey and purple dashed lines, respectively
      (<a href="https://ui.adsabs.harvard.edu/abs/2025ApJ...994L..45F/abstract">Franz et&nbsp;al. 2025</a>).
      </figcaption>
    </figure>
  </div>

  <div class="project__body">
    <span class="eyebrow">Multi-messenger astrophysics &middot; SAGUARO &middot; TROVE</span>
    <h2 class="project__title">Gravitational-wave follow-up: finding the light</h2>

    <p>
      A LIGO&ndash;Virgo&ndash;KAGRA alert arrives with a localisation covering hundreds of
      square degrees, a few dozen plausible host galaxies, and a kilonova that fades in
      days. Turning that into an identified counterpart is a problem of triage under time
      pressure, and just as much a problem of knowing what the contaminants look like.
      Most of what you find in a localisation volume is not a kilonova.
    </p>

    <h3>SAGUARO</h3>
    <p>
      I work within <a href="https://saguaro-mma.github.io/">SAGUARO</a> (Searches After
      Gravitational waves Using ARizona Observatories), which turns Arizona's telescopes
      into a rapid-response network for compact-object mergers. Alongside it I am
      PI of dedicated <strong>MMT</strong> and <strong>Magellan</strong> programs at Steward
      for O4 and O4-IR1 follow-up, giving the collaboration guaranteed spectroscopic and
      imaging time to characterise candidates rather than merely detect them. Deciding which
      of thirty candidates gets the next hour on a 6.5-metre telescope, at three in the
      morning, is the actual job.
    </p>

    <h3>TROVE</h3>
    <p>
      Candidate vetting is where these searches succeed or fail, and it does not scale by
      hand. I contribute to <strong>TROVE</strong> (the Tool for Rapid Object Vetting and
      Examination), which ingests alert-stream candidates and surfaces the
      information a human needs to make a fast, defensible call: host association, archival
      history, cross-survey photometry, and the discriminants that separate a kilonova from a
      young supernova or a nuclear flare. I also coordinate through
      <strong>AZTEC</strong> and the LSST Discovery Alliance TVS&ndash;LVK effort, which is
      where this becomes a Rubin-era problem: the same alert volume, a much larger haystack.
    </p>

    <h3>What this has produced</h3>
    <p>
      The Type&nbsp;IIb <strong>SN&nbsp;2025ulz</strong> is the clearest example. It sat in
      the localisation volume of the low-significance event S250818k, looked briefly like a
      kilonova, and turned out to be a supernova. That is the ambiguity you have to settle
      quickly <em>and</em> correctly, because a wrong call propagates through every
      follow-up decision that comes after it. We also searched for a counterpart to the
      subsolar-mass candidate <strong>S251112cm</strong>, a signal that would be hard to
      explain with any ordinary compact object.
    </p>


    <div class="links">
      <a href="https://ui.adsabs.harvard.edu/abs/2025ApJ...994L..45F/abstract">SN 2025ulz (ADS)</a>
      <a href="https://arxiv.org/abs/2510.17104">arXiv:2510.17104</a>
      <a href="https://arxiv.org/abs/2603.17009">S251112cm (arXiv:2603.17009)</a>
      <a href="https://saguaro-mma.github.io/">SAGUARO</a>
      <a href="http://sand.as.arizona.edu/saguaro_tom/">SAGUARO TOM</a>
      <a href="https://datatrove-test.as.arizona.edu/">TROVE</a>
    </div>
  </div>
</section>

<!-- ───────────────────────── 5. REFITT ─────────────────────── -->
<section class="project" id="refitt">
  <figure class="project__figure project__figure--plate">
    <img src="{{ '/images/Science_Follow_up.png' | relative_url }}"
         alt="REFITT characterisation of transients from grids of core-collapse simulations, and recommended follow-up epochs for ZTF22aaacxkp"
         loading="lazy" decoding="async">
    <figcaption>
      <strong>Left:</strong> REFITT uses grids of core-collapse simulations to characterise
      ZTF transients on the fly, returning kinetic energy, mass-loss rate,
      <sup>56</sup>Ni mass and ejecta mass to guide decisions.
      <strong>Right:</strong> follow-up of the Type&nbsp;II ZTF22aaacxkp at
      REFITT-recommended epochs (diamonds)
      (<a href="https://iopscience.iop.org/article/10.3847/1538-4357/aca80a">Subrayan et&nbsp;al. 2023</a>).
    </figcaption>
  </figure>

  <div class="project__body">
    <span class="eyebrow">AI for all-sky surveys</span>
    <h2 class="project__title">Science-driven forecasts for transient follow-up</h2>

    <p>
      The Rubin Observatory will report millions of alerts per night against a global
      spectroscopic capacity that is essentially fixed. The scarce resource is not
      detection. It is deciding which objects deserve a telescope, and on which night.
    </p>

    <p>
      The <a href="https://refitt.physics.purdue.edu/">Recommender Engine for Intelligent
      Transient Tracking (REFITT)</a> attacks that by prioritising follow-up on physical
      grounds. I showed that pre-computed hydrodynamical model grids combined with
      statistical inference can characterise a core-collapse supernova while it is still
      rising, recovering progenitor and explosion parameters from sparse ZTF light curves,
      and then identify the epochs where one extra observation actually changes the
      answer. That turns follow-up from
      first-come-first-served into something closer to an optimisation problem.
    </p>

    <div class="links">
      <a href="https://ui.adsabs.harvard.edu/abs/2023ApJ...945...46S/abstract">ADS</a>
      <a href="https://arxiv.org/abs/2211.15702">arXiv:2211.15702</a>
      <a href="https://iopscience.iop.org/article/10.3847/1538-4357/aca80a">ApJ</a>
      <a href="https://ui.adsabs.harvard.edu/abs/2023PASJ...75..634M/abstract">Model grid (Moriya+ 2023)</a>
    </div>
  </div>
</section>

<!-- ──────────────────── 7. PREPARING FOR LSST ──────────────── -->
<section class="project" id="lsst-era">
  <figure class="project__figure">
    <img src="{{ '/images/rubin_era_night_sky.jpg' | relative_url }}"
         alt="A telescope dome on a mountain ridge beneath the arc of the Milky Way"
         loading="lazy" decoding="async">
    <!-- TODO: name the facility in the caption and add the photographer's credit. -->
    <figcaption>
      The southern sky from the mountaintop. Rubin, and the surveys shadowing it, will
      turn this view into millions of alerts a night.
    </figcaption>
  </figure>

  <div class="project__body">
    <span class="eyebrow">Surveys &middot; Instrumentation</span>
    <h2 class="project__title">Getting ready for the Rubin era</h2>

    <p>
      Much of what I do is infrastructure for the next decade: building the discovery and
      follow-up channels that early-time and late-time transient science will both depend
      on. I am a co-investigator on <strong>SHADOW</strong>, the DECam survey shadowing
      Rubin/LSST to find the youngest transients in the nearby universe, and on
      <strong>PASSTA</strong>, the public AEON spectroscopic survey for transient astronomy
      on SOAR. I work within DLT40, the Global Supernova
      Project, TROVE and the ULTRASAT collaboration, and I have contributed to
      commissioning the new 90-inch instrument on the Bok telescope at Steward.
    </p>

    <p>
      The first result from the LSST shadow survey, the restless luminous blue variable
      AT&nbsp;2017des in NGC&nbsp;4532, shows what shadowing buys you: a well-sampled
      record of a star behaving badly for years before anything definitive happens to
      it.
    </p>

    <div class="links">
      <a href="https://arxiv.org/abs/2606.23784">SHADOW first results (arXiv:2606.23784)</a>
      <a href="{{ '/talks/' | relative_url }}">Telescope programs</a>
    </div>
  </div>
</section>

<!--
  ══════════════════════════════════════════════════════════════
  FIGURES & PLOTS
  ──────────────────────────────────────────────────────────────
  The gallery below builds itself from _data/gallery.yml: add a
  plot there and it appears here. If that list is empty the whole
  section disappears, so it is safe to leave this line in place.
  ══════════════════════════════════════════════════════════════
-->
{% include gallery.html %}
