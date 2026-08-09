---
layout: home
title: Home
---

<div id="intro-wrapper" class="l-text">
	<div id="intro-title-wrapper">
		<div id="intro-image-wrapper">
			<img id="intro-image" src="/images/portrait.jpg"></div>
		<div id="intro-title-text-wrapper">
			<h1 id="intro-title">Hi, I'm Weiran Yao</h1>
			<div id="intro-subtitle">I'm Co-Founder & Chief AI Officer</div>
			<div id="intro-subtitle">at actAVA</div>
			<div id="intro-title-socials">
				{% for link in site.data.social-links %}
					{% if link.on-homepage == true %}
						{% include social-link.html link=link %}
					{% endif %}
				{% endfor %}
			</div>
		</div>
	</div>
	<!-- <hr class="l-middle home-hr"> -->
	<div id="everything-else" class="l-middle">
		<a href="{{ site.url }}/cv"><div><i class="fa fa-portrait icon icon-right-space"></i>CV</div></a>
		<a href="{{ site.url }}/projects"><div><i class="fa fa-shapes icon icon-right-space"></i>Projects</div></a>
		<a href="{{ site.url }}/everything-else"><div><i class="fa fa-list-ul icon icon-right-space"></i>Everything Else</div></a>
	</div>
	<div>
		I build <span class="cv-vis"><b>multi-agent AI systems</b></span> and train the <span class="cv-ai"><b>frontier models</b></span> underneath them.
	</div>
	<div style="height: 1rem"></div>
	<div>
		I co-founded <img class="intro-logo" style="height: 15px; width: auto; padding-bottom: 2px;" src="/images/actava-icon.svg"> <a href="https://www.actava.ai/"><b>actAVA</b></a> and own its AI organization. We give healthcare enterprises <span class="cv-vis">agentic sovereignty</span> — the ability to build, test, and own their AI agents rather than rent someone else's.
	</div>
	<div style="height: 1rem"></div>
	<div>
		I lead post-training of <a href="/papers/cura"><span class="cv-ai">Cura 1T</span></a>, our trillion-parameter healthcare model, trained through a <span class="cv-ai">recursive self-improvement</span> loop in which a training agent finds the model's capability gaps and closes them with SFT, RL, and self-distillation. Cura ranks at or near the top of frontier baselines on five of six healthcare evaluation panels while holding its out-of-domain reasoning.
	</div>
	<div style="height: 1rem"></div>
	<div>
		I also lead <a href="/papers/chi-bench"><span class="cv-vis">χ-Bench</span></a>, our benchmark for long-horizon, policy-rich clinical workflows, where the best frontier agent resolves only 28% of tasks. On the platform side I work on <a href="https://www.actava.ai/products"><span class="cv-vis">KORA</span></a>, a model-independent harness for building, testing, and continually improving agents, and <a href="https://www.actava.ai/chryso"><span class="cv-vis">CHRYSO</span></a>, which enforces AI governance against 85+ regulatory controls.
	</div>
	<div style="height: 1rem"></div>
	<div>
		Previously at <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/salesforce.svg"> Salesforce AI Research, I led the <span class="cv-ai">post-training team</span>. We shipped <a href="/papers/xlam"><span class="cv-ai">xLAM</span></a>, a family of state-of-the-art function-calling models, the synthetic data pipelines behind <a href="/papers/apigen"><span class="cv-ai">APIGen</span></a>, <a href="/papers/apigenmt"><span class="cv-ai">APIGen-MT</span></a>, and <a href="/papers/agent-ohana"><span class="cv-ai">AgentOhana</span></a>, and <a href="/papers/retroformer"><span class="cv-ai">Retroformer</span></a>, a generative critic model for self-reflection.
	</div>
	<div style="height: 1rem"></div>
	<div>
		I also built agent systems there, including <a href="/blog/slack-agents"><span class="cv-vis">SlackAgents</span></a>, <a href="/papers/agentlite"><span class="cv-vis">AgentLite</span></a>, <a href="https://engineering.salesforce.com/codegenie-how-salesforce-leveraged-generative-ai-to-enhance-internal-developer-productivity/?utm_source=socialshare&utm_medium=organic_social&utm_campaign=amer_sfjobs_sfteaw&utm_content=graphic&blaid=6592267"><span class="cv-vis">CodeGenie</span></a>, <a href="/papers/dei"><span class="cv-vis">SWE Agents</span></a>, and <a href="/blog/aiops"><span class="cv-vis">AIOps</span></a> for cloud incident causation analysis.
	</div>
	<div style="height: 1rem"></div>
	<div>
		I did my Ph.D. and M.S. in Machine Learning at <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/cmu.png"> CMU, focusing on model interpretability, where I was advised by <a href="https://www.andrew.cmu.edu/user/kunz1/index.html">Dr. Kun Zhang</a>.
	</div>
</div>

<hr class="l-middle home-hr">

<h2 class="feature-title">Featured <a href="/cv/#publications">Research Publications</a></h2>

<p class="feature-text">
	Latest research for fans of AI Agent, RL and Interpretability.
</p>

<div class="cover-wrapper cover-wrapper-3-col l-page">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>

<br>

<h2 class="feature-title">Featured <a href="/cv/#engineering-projects">Engineering Projects</a></h2>

<p class="feature-text">
	Innovative AI systems I've developed and deployed at scale.
</p>

<div class="cover-wrapper cover-wrapper-3-col l-page">
	{% assign sortedArticles = site.data.articles | where: "featured", true % | sort: 'feature-order' %}
	{% for feature in sortedArticles %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>

<br>
<h2 class="feature-title">Featured <a href="/cv/#press">Talks & Presentations</a></h2>

<p class="feature-text">
	My favorite talks and presentations given at industry AI conferences and workshops.
</p>

<div class="cover-wrapper cover-wrapper-3-col l-page">
	{% assign sortedTalks = site.data.talks | where: "featured", true % | sort: 'feature-order' %}
	{% for feature in sortedTalks %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>



[gt]: http://www.gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "Georgia Tech Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "Georgia Tech College of Computing"

[cv]: {{ site.url }}/cv
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau"
[alex]: http://va.gatech.edu/endert/ "Alex Endert"
[poloclub]: http://poloclub.gatech.edu "Polo Club of Data Science"
[nstrf]: https://www.nasa.gov/strg/nstrf "NASA Space Technology Research Fellowship"