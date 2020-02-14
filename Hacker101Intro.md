---


---

<h1 id="hacker-one-introduction">Hacker One Introduction</h1>
<h2 id="what-i-will-learn">What I will learn:</h2>
<ul>
<li>How to identify, exploit, and remediate the top web security vulnerabilities, as well as many more arcane bugs.</li>
<li>How to properly handle cryptography.</li>
<li>How to design and review applications from a security standpoint.</li>
<li>How to operate as a bug bounty hunter or security consultant.</li>
<li>Much More.</li>
</ul>
<p>Learn about web request with Python ‘request’ package.</p>
<h2 id="must-have-tools">Must-Have Tools</h2>
<ul>
<li>Burp Proxy
<ol>
<li>This allow you to watch HTTPS(s) communication, intercept and modify request, and replay existing request.</li>
<li>You will use this constantly in both your coursework and exams.</li>
</ol>
</li>
<li>Firefox
<ol>
<li>Firefox allows you to set proxy settings specificaly in the browser, rather than setting them system-wide.</li>
<li>This will be your friend when you’re testing, to isolate an application.</li>
</ol>
</li>
</ul>
<h1 id="introduction-to-security">Introduction to Security</h1>
<p>You’re here to break things before anyone else does, so that vulneravilities can be fixed before attackers get to them.</p>
<p>To do that, you need to understand how attackers operate what their goals are, and how they think.</p>
<h2 id="thinking-like-a-breaker">Thinking like a breaker</h2>
<p>The most important tenet of the breaker mindset is this: pushing a button is the most effective way to discover what it does.</p>
<p>If you don’t understand what an application is doing and why it’s doing it, you’re goint to have a hard time finding ways to break it.</p>
<h2 id="imbalance">Imbalance</h2>
<p>The key difference between defending and attacking is this:</p>
<p>Defenders have to find every bug; attackers only need to find a few.</p>
<p>This means that attackers will always have the advantage over defenders.</p>
<h2 id="attacker-goals">Attacker Goals</h2>
<p>When accessing an application, find every bit of functionality you can. Once you have a rough list of all the bits of the application,<br>
consider this: if I was an attacker, what would my goal be?</p>
<p>Maybe I´d want credit card number from an ecommerce site, maybe I´d want to destroy or falsify data in a server monitoring application.</p>
<h2 id="prioritization">Prioritization</h2>
<p>Once you have a good picture of what an attacker might want, you can start to rank areas of the application in terms of payoff: if I compromise<br>
area X, does that give me low-value information of high-value? What about Y instead?</p>
<p>When possible, asking developers the question “what keeps you up at night?” will often point to check.</p>
<h2 id="reports">Reports</h2>
<p>Is a critical skill of communicating with developers clientes and other hackers, will affect</p>
<p>the value of your findings more than almost anything else.</p>
<p>For the purposes of this course and for most bug reporting you’ll do in general you’re going to include the following for each bug:</p>
<ul>
<li>Title – E.g “Reflected Cross-Site Scripting in Profiles”</li>
<li>Severity</li>
<li>Description – Brief description of what the vulnerability if.</li>
<li>Reproduction Septs – Brief description of how to reproduce the bug; preferably with a small proof of concept.</li>
<li>Impact – What cen be done with the vulnerability?</li>
<li>Mitigation – How is it fixed?</li>
<li>Affected Assets – Generally a list of affected URLs.</li>
</ul>
<h3 id="severity">Severity</h3>
<p>This is handled differently just about everywhere, but I recommend basing severity on difficulty of explotation and potential business impact.<br>
The following ranking are what I use:</p>
<ul>
<li><strong>Informational</strong> – Issue has no real impact.</li>
<li><strong>Low</strong> – The business impact is minimal.</li>
<li><strong>Medium</strong> – Potential to cause harm to users, but not revealing any critical data.</li>
<li><strong>High</strong> – Potential to reveal user data or aids in explotation of other important vulnerabilities.</li>
<li><strong>Critical</strong>  – High risk of personal/confidential data exposure, general system compromise, and other situations with severe business impact.</li>
</ul>
<h2 id="reflected-xss-first-bug-example">Reflected XSS First Bug Example</h2>
<p>What you’ve just seen is an example of reflected cross-site scripting (a.k.a Reflected XSS or rXSS)<br>
In essence, a parameter that an attacker controls is directly reflected back to a user. This could allow injection of raw HTML<br>
or JavaScript (depending on where the XSS takes place) and allow an attacker to perform actions in the context of another user.</p>
<p>This is obviously a contrived example and we’ll cover much more in terms of XSS in the next couple sessions. But think about all the places<br>
where you input gets reflected on a website on a daily basis.</p>
<p>How many of those inputs are vulnerable? How many will safety sanitize the data? You’d be surprised.</p>
<h2 id="next-session">Next Session</h2>
<p>Next session we’ll be getting deep into how browsers and the web in general work. You’ll also learn about Cross Site Request Forgery,<br>
one of the most common and important vulnerabilities.</p>
<p>For now, get your proxy setup and play round with it – take a look  at the flow of data when your browse to several sites.</p>
<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>

