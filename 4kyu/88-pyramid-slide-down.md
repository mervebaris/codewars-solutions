### Problem:
<h3 id="lyrics">Lyrics...</h3>
<p>Pyramids are amazing! Both in architectural and mathematical sense. If you have a computer, you can mess with pyramids even if you are not in Egypt at the time. For example, let&apos;s consider the following problem. Imagine that you have a pyramid built of numbers, like this one here:</p>
<pre><code>   /3/
  \7\ 4 
 2 \4\ 6 
8 5 \9\ 3</code></pre><h3 id="here-comes-the-task">Here comes the task...</h3>
<p>Let&apos;s say that the <em>&apos;slide down&apos;</em> is a sum of consecutive numbers from the top to the bottom of the pyramid. As you can see, the longest <em>&apos;slide down&apos;</em> is <code>3 + 7 + 4 + 9 = 23</code></p>
<p>Your task is to write a function <code>longestSlideDown</code> (in ruby: <code>longest_slide_down</code>) that takes a pyramid representation as argument and returns its&apos; <strong>longest</strong> <em>&apos;slide down&apos;</em>. For example,</p>
<pre><code class="language-haskell"><span class="hljs-title">longestSlideDown</span> [[<span class="hljs-number">3</span>], [<span class="hljs-number">7</span>, <span class="hljs-number">4</span>], [<span class="hljs-number">2</span>, <span class="hljs-number">4</span>, <span class="hljs-number">6</span>], [<span class="hljs-number">8</span>, <span class="hljs-number">5</span>, <span class="hljs-number">9</span>, <span class="hljs-number">3</span>]]  -&gt; <span class="hljs-number">23</span></code></pre>
<pre style="display: none;"><code class="language-python">longestSlideDown([[3], [7, 4], [2, 4, 6], [8, 5, 9, 3]]) =&gt; 23</code></pre>
<pre style="display: none;"><code class="language-javascript">longestSlideDown([[<span class="hljs-number">3</span>], [<span class="hljs-number">7</span>, <span class="hljs-number">4</span>], [<span class="hljs-number">2</span>, <span class="hljs-number">4</span>, <span class="hljs-number">6</span>], [<span class="hljs-number">8</span>, <span class="hljs-number">5</span>, <span class="hljs-number">9</span>, <span class="hljs-number">3</span>]]) =&gt; <span class="hljs-number">23</span></code></pre>
<pre style="display: none;"><code class="language-ruby">longest_slide_down([[<span class="hljs-number">3</span>], [<span class="hljs-number">7</span>, <span class="hljs-number">4</span>], [<span class="hljs-number">2</span>, <span class="hljs-number">4</span>, <span class="hljs-number">6</span>], [<span class="hljs-number">8</span>, <span class="hljs-number">5</span>, <span class="hljs-number">9</span>, <span class="hljs-number">3</span>]]) =&gt; <span class="hljs-number">23</span></code></pre>
<pre style="display: none;"><code class="language-java">longestSlideDown [[<span class="hljs-number">3</span>], [<span class="hljs-number">7</span>, <span class="hljs-number">4</span>], [<span class="hljs-number">2</span>, <span class="hljs-number">4</span>, <span class="hljs-number">6</span>], [<span class="hljs-number">8</span>, <span class="hljs-number">5</span>, <span class="hljs-number">9</span>, <span class="hljs-number">3</span>]] =&gt; <span class="hljs-number">23</span></code></pre>
<pre style="display: none;"><code class="language-clojure">(longestSlideDown [[3] [7 4] [2 4 6] [8 5 9 3]]) =&gt; 23</code></pre>
<pre style="display: none;"><code class="language-csharp">LongestSlideDown(<span class="hljs-keyword">new</span>[] { <span class="hljs-keyword">new</span>[] {<span class="hljs-number">3</span>}, <span class="hljs-keyword">new</span>[] {<span class="hljs-number">7</span>, <span class="hljs-number">4</span>}, <span class="hljs-keyword">new</span>[] {<span class="hljs-number">2</span>, <span class="hljs-number">4</span>, <span class="hljs-number">6</span>}, <span class="hljs-keyword">new</span>[] {<span class="hljs-number">8</span>, <span class="hljs-number">5</span>, <span class="hljs-number">9</span>, <span class="hljs-number">3</span>} }); =&gt; <span class="hljs-number">23</span></code></pre>
<h3 id="by-the-way">By the way...</h3>
<p>My tests include some extraordinarily high pyramides so as you can guess, brute-force method is a bad idea unless you have a few centuries to waste. You must come up with something more clever than that.</p>
<p>(c) This task is a lyrical version of the <strong>Problem 18</strong> and/or <strong>Problem 67</strong> on <a href="https://projecteuler.net" target="_blank">ProjectEuler</a>.</p>

### Solution