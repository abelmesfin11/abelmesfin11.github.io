---
layout: page
permalink: /projects/
title: projects
description: course projects and things I've built
nav: true
nav_order: 3
---

<style>
  .proj { margin-bottom: 1.1rem; }
  .proj .tech { color: var(--global-text-color-light); font-size: .9rem; }
</style>

{% assign gh = "https://github.com/abelmesfin11/" %}

<h3>machine learning & causal inference</h3>

<p class="proj"><b>Covariate adjustment for MNAR data</b> <span class="tech">· Python</span> <a href="{{ gh }}Covariate-Adjustment-for-MNAR-data">[code]</a><br>
Implemented <a href="https://arxiv.org/abs/1907.01654">Saadati & Tian's</a> adjustment criterion for controlling confounding when data is missing not at random.</p>

<p class="proj"><b>Drought and support for political violence in Kenya</b> <span class="tech">· Python</span> <a href="{{ gh }}CSCI379-Causal-Inference-Final-Project">[code]</a><br>
Revisited an associational study with causal inference methods and found no evidence of a causal effect.</p>

<p class="proj"><b>Neural network from scratch</b> <span class="tech">· Python, NumPy</span> <a href="{{ gh }}customerRetention">[code]</a><br>
Implemented autograd, backpropagation, and dropout without ML frameworks; 93% accuracy on customer churn prediction.</p>

<p class="proj"><b>Decision tree and logistic regression from scratch</b> <span class="tech">· Python, NumPy</span> <a href="{{ gh }}Custom-Decision-Tree-Classifier">[tree]</a> <a href="{{ gh }}Logistic-Regression-Engine">[logistic]</a><br>
Classifiers built without ML libraries and applied to clinical datasets.</p>

<h3>distributed & systems</h3>

<p class="proj"><b>Multithreaded web server</b> <span class="tech">· C, pthreads</span><br>
An HTTP/1.0 and 1.1 server that handles each client on its own thread and supports persistent connections.</p>

<p class="proj"><b>TinyBookstore</b> <span class="tech">· Java, XML-RPC, SQLite</span> <a href="{{ gh }}TinyBookstore">[code]</a><br>
A client/server bookstore with remote search, lookup, and purchase operations.</p>

<p class="proj"><b>Cache simulator</b> <span class="tech">· C</span> <a href="{{ gh }}cache-simulator">[code]</a><br>
Simulates a set-associative cache with LRU replacement over real memory traces.</p>

<h3>web & apps</h3>

<p class="proj"><b>Movie recommendation engine</b> <span class="tech">· Next.js, TypeScript, Postgres</span><br>
A personalized "For You" feed for a movie and TV discovery app that ranks titles from viewing history.</p>

<p class="proj"><b>Spotalyze</b> <span class="tech">· React, Node.js, Express</span> <a href="{{ gh }}spotify-wrap-app">[code]</a><br>
A Spotify analytics app showing top tracks, artists, and playlist audio features.</p>

<p class="proj"><b>Little Bistro</b> <span class="tech">· Django REST Framework</span> <a href="{{ gh }}little-bistro">[code]</a><br>
A restaurant web app and REST API for menus, carts, and orders.</p>

<p>More on my <a href="https://github.com/abelmesfin11">GitHub</a>.</p>
