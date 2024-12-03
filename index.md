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
			<div id="intro-subtitle">I'm a Senior Research Scientist & Manager</div>
			<div id="intro-subtitle">at Salesforce AI Research</div>
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
		I develop <span class="cv-vis"><b>multi-agent AI systems</b></span> and train their <span class="cv-ai"><b>language models</b></span>.
	</div>
	<div style="height: 1rem"></div>
	<div>
		At <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/salesforce.svg"> Salesforce, I work on AI agent systems including <a href="/blog/slack-agents"><span class="cv-vis">SlackAgents</span></a>, <a href="/papers/agentlite"><span class="cv-vis">AgentLite</span></a>, <a href="https://engineering.salesforce.com/codegenie-how-salesforce-leveraged-generative-ai-to-enhance-internal-developer-productivity/?utm_source=socialshare&utm_medium=organic_social&utm_campaign=amer_sfjobs_sfteaw&utm_content=graphic&blaid=6592267"><span class="cv-vis">CodeGenie</span></a>, <a href="/papers/dei"><span class="cv-vis">SWE Agents</span></a>, and <a href="https://www.loom.com/share/408133a7a8e14208842afbe1c140727c?sid=fd6d0181-a52b-4acd-82a7-7831bd26dcbe"><span class="cv-vis">WebAgent</span></a>.
	</div>
	<div style="height: 1rem"></div>
	<div>
		For models, I've led post-training of <a href="/papers/retroformer"><span class="cv-ai">Retroformer</span></a>, a genertive critic model for self-reflection. I've worked on <a href="/papers/xlam"><span class="cv-ai">xLAM</span></a>, a family of state-of-the-art language models for function calling. I conducted research on synthetic data generation pipeline for <a href="/papers/apigen"><span class="cv-ai">APIGen</span></a> and <a href="/papers/agent-ohana"><span class="cv-ai">AgentOhana</span></a>.
	</div>
	<div style="height: 1rem"></div>
	<div>
		For products, I've led delevopment of <a href="/blog/aiops"><span class="cv-vis">AIOps</span></a> for cloud incident causation analysis, enhancing operational efficiency on Salesforce Availability Cloud. I worked on <span class="cv-vis">function call</span> and <span class="cv-vis">structured output</span> API endpoints of Salesforce xLAM services.
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

<h2 class="feature-title">Featured <a href="/cv/#interactive-articles">Engineering Projects</a></h2>

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
<h2 class="feature-title">Featured <a href="https://parametric.press/about">Talks & Presentations</a></h2>

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