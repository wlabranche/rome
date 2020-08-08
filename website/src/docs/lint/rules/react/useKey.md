<<<<<<< HEAD:website/src/docs/lint/rules/react/jsxKey.md
---
title: Lint Rule react/jsxKey
layout: layouts/rule.liquid
description: This rule detects a missing `key` prop
eleventyNavigation:
	key: lint-rules/react/jsxKey
	parent: lint-rules
	title: react/jsxKey
---

# react/jsxKey

This rule detects a missing `key` prop in a element that requires it. Keys help React identify which items have changed, are added, or are removed.
=======
---
title: Lint Rule react/useKey
layout: layouts/rule.liquid
description: MISSING DOCUMENTATION
eleventyNavigation:
	key: lint-rules/react/useKey
	parent: lint-rules
	title: react/useKey
---

# react/useKey

MISSING DOCUMENTATION
>>>>>>> feat: consolidate lint rule naming:website/src/docs/lint/rules/react/useKey.md

<!-- GENERATED:START(hash:3651704e32323addd9d0679a6a3021f7aeaaa6f9,id:main) Everything below is automatically generated. DO NOT MODIFY. Run `./rome run scripts/generated-files/lint-rules-docs` to update. -->
## Examples
### Invalid
{% raw %}<pre class="language-text"><code class="language-text"><span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span>&lt;<span class="token attr-name">div</span> <span class="token operator">/</span>&gt;<span class="token punctuation">,</span> &lt;<span class="token attr-name">div</span> <span class="token operator">/</span>&gt;<span class="token punctuation">]</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text">
 <span style="text-decoration-style: dashed; text-decoration-line: underline;">file.tsx:1:11</span> <strong>lint/react/useKey</strong> ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  <strong><span style="color: Tomato;">✖ </span></strong><span style="color: Tomato;">Provide a </span><span style="color: Tomato;"><strong>key</strong></span><span style="color: Tomato;"> prop with a unique value for each element in </span><span style="color: Tomato;"><strong>array</strong></span><span style="color: Tomato;">.</span>

    <span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span>&lt;<span class="token attr-name">div</span> <span class="token operator">/</span>&gt;<span class="token punctuation">,</span> &lt;<span class="token attr-name">div</span> <span class="token operator">/</span>&gt;<span class="token punctuation">]</span>
               <span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span>

  <strong><span style="color: DodgerBlue;">ℹ </span></strong><span style="color: DodgerBlue;">Keys help React identify which items have changed, are added, or are</span>
    <span style="color: DodgerBlue;">removed.</span>

 <span style="text-decoration-style: dashed; text-decoration-line: underline;">file.tsx:1:20</span> <strong>lint/react/useKey</strong> ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  <strong><span style="color: Tomato;">✖ </span></strong><span style="color: Tomato;">Provide a </span><span style="color: Tomato;"><strong>key</strong></span><span style="color: Tomato;"> prop with a unique value for each element in </span><span style="color: Tomato;"><strong>array</strong></span><span style="color: Tomato;">.</span>

  <strong><span style="color: DodgerBlue;">ℹ </span></strong><span style="color: DodgerBlue;">Keys help React identify which items have changed, are added, or are</span>
    <span style="color: DodgerBlue;">removed.</span>

</code></pre>{% endraw %}

---------------

{% raw %}<pre class="language-text"><code class="language-text"><span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">x</span> <span class="token operator">=&gt;</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text">
 <span style="text-decoration-style: dashed; text-decoration-line: underline;">file.tsx:1:26</span> <strong>lint/react/useKey</strong> ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  <strong><span style="color: Tomato;">✖ </span></strong><span style="color: Tomato;">Provide a </span><span style="color: Tomato;"><strong>key</strong></span><span style="color: Tomato;"> prop with a unique value for each element in </span><span style="color: Tomato;"><strong>iterator</strong></span><span style="color: Tomato;">.</span>

    <span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">x</span> <span class="token operator">=&gt;</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">)</span><span class="token punctuation">;</span>
                              <span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span>

  <strong><span style="color: DodgerBlue;">ℹ </span></strong><span style="color: DodgerBlue;">Keys help React identify which items have changed, are added, or are</span>
    <span style="color: DodgerBlue;">removed.</span>

</code></pre>{% endraw %}

---------------

{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">React</span><span class="token punctuation">.</span><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text">
 <span style="text-decoration-style: dashed; text-decoration-line: underline;">file.tsx:1:34</span> <strong>lint/react/useKey</strong> ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  <strong><span style="color: Tomato;">✖ </span></strong><span style="color: Tomato;">Provide a </span><span style="color: Tomato;"><strong>key</strong></span><span style="color: Tomato;"> prop with a unique value for each element in </span><span style="color: Tomato;"><strong>iterator</strong></span><span style="color: Tomato;">.</span>

    <span class="token variable">React</span><span class="token punctuation">.</span><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">)</span><span class="token punctuation">;</span>
                                      <span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span>

  <strong><span style="color: DodgerBlue;">ℹ </span></strong><span style="color: DodgerBlue;">Keys help React identify which items have changed, are added, or are</span>
    <span style="color: DodgerBlue;">removed.</span>

</code></pre>{% endraw %}

---------------

{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text">
 <span style="text-decoration-style: dashed; text-decoration-line: underline;">file.tsx:1:28</span> <strong>lint/react/useKey</strong> ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  <strong><span style="color: Tomato;">✖ </span></strong><span style="color: Tomato;">Provide a </span><span style="color: Tomato;"><strong>key</strong></span><span style="color: Tomato;"> prop with a unique value for each element in </span><span style="color: Tomato;"><strong>iterator</strong></span><span style="color: Tomato;">.</span>

    <span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">)</span><span class="token punctuation">;</span>
                                <span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span>

  <strong><span style="color: DodgerBlue;">ℹ </span></strong><span style="color: DodgerBlue;">Keys help React identify which items have changed, are added, or are</span>
    <span style="color: DodgerBlue;">removed.</span>

</code></pre>{% endraw %}

---------------

{% raw %}<pre class="language-text"><code class="language-text"><span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">x</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text">
 <span style="text-decoration-style: dashed; text-decoration-line: underline;">file.tsx:2:8</span> <strong>lint/react/useKey</strong> ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  <strong><span style="color: Tomato;">✖ </span></strong><span style="color: Tomato;">Provide a </span><span style="color: Tomato;"><strong>key</strong></span><span style="color: Tomato;"> prop with a unique value for each element in </span><span style="color: Tomato;"><strong>iterator</strong></span><span style="color: Tomato;">.</span>

  <strong>  1</strong><strong> │ </strong><span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">x</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>
  <strong><span style="color: Tomato;">&gt;</span></strong><strong> 2</strong><strong> │ </strong>  <span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
     <strong> │ </strong>         <span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span>
  <strong>  3</strong><strong> │ </strong><span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

  <strong><span style="color: DodgerBlue;">ℹ </span></strong><span style="color: DodgerBlue;">Keys help React identify which items have changed, are added, or are</span>
    <span style="color: DodgerBlue;">removed.</span>

</code></pre>{% endraw %}

---------------

{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">React</span><span class="token punctuation">.</span><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text">
 <span style="text-decoration-style: dashed; text-decoration-line: underline;">file.tsx:2:8</span> <strong>lint/react/useKey</strong> ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  <strong><span style="color: Tomato;">✖ </span></strong><span style="color: Tomato;">Provide a </span><span style="color: Tomato;"><strong>key</strong></span><span style="color: Tomato;"> prop with a unique value for each element in </span><span style="color: Tomato;"><strong>iterator</strong></span><span style="color: Tomato;">.</span>

  <strong>  1</strong><strong> │ </strong><span class="token variable">React</span><span class="token punctuation">.</span><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>
  <strong><span style="color: Tomato;">&gt;</span></strong><strong> 2</strong><strong> │ </strong>  <span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
     <strong> │ </strong>         <span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span>
  <strong>  3</strong><strong> │ </strong><span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

  <strong><span style="color: DodgerBlue;">ℹ </span></strong><span style="color: DodgerBlue;">Keys help React identify which items have changed, are added, or are</span>
    <span style="color: DodgerBlue;">removed.</span>

</code></pre>{% endraw %}

---------------

{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text">
 <span style="text-decoration-style: dashed; text-decoration-line: underline;">file.tsx:2:8</span> <strong>lint/react/useKey</strong> ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  <strong><span style="color: Tomato;">✖ </span></strong><span style="color: Tomato;">Provide a </span><span style="color: Tomato;"><strong>key</strong></span><span style="color: Tomato;"> prop with a unique value for each element in </span><span style="color: Tomato;"><strong>iterator</strong></span><span style="color: Tomato;">.</span>

  <strong>  1</strong><strong> │ </strong><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>
  <strong><span style="color: Tomato;">&gt;</span></strong><strong> 2</strong><strong> │ </strong>  <span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
     <strong> │ </strong>         <span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span>
  <strong>  3</strong><strong> │ </strong><span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

  <strong><span style="color: DodgerBlue;">ℹ </span></strong><span style="color: DodgerBlue;">Keys help React identify which items have changed, are added, or are</span>
    <span style="color: DodgerBlue;">removed.</span>

</code></pre>{% endraw %}

---------------

{% raw %}<pre class="language-text"><code class="language-text"><span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token keyword">function</span><span class="token punctuation">(</span><span class="token variable">x</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text">
 <span style="text-decoration-style: dashed; text-decoration-line: underline;">file.tsx:2:8</span> <strong>lint/react/useKey</strong> ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  <strong><span style="color: Tomato;">✖ </span></strong><span style="color: Tomato;">Provide a </span><span style="color: Tomato;"><strong>key</strong></span><span style="color: Tomato;"> prop with a unique value for each element in </span><span style="color: Tomato;"><strong>iterator</strong></span><span style="color: Tomato;">.</span>

  <strong>  1</strong><strong> │ </strong><span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token keyword">function</span><span class="token punctuation">(</span><span class="token variable">x</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
  <strong><span style="color: Tomato;">&gt;</span></strong><strong> 2</strong><strong> │ </strong>  <span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
     <strong> │ </strong>         <span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span>
  <strong>  3</strong><strong> │ </strong><span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

  <strong><span style="color: DodgerBlue;">ℹ </span></strong><span style="color: DodgerBlue;">Keys help React identify which items have changed, are added, or are</span>
    <span style="color: DodgerBlue;">removed.</span>

</code></pre>{% endraw %}

---------------

{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">React</span><span class="token punctuation">.</span><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token keyword">function</span><span class="token punctuation">(</span><span class="token variable">x</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text">
 <span style="text-decoration-style: dashed; text-decoration-line: underline;">file.tsx:2:8</span> <strong>lint/react/useKey</strong> ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  <strong><span style="color: Tomato;">✖ </span></strong><span style="color: Tomato;">Provide a </span><span style="color: Tomato;"><strong>key</strong></span><span style="color: Tomato;"> prop with a unique value for each element in </span><span style="color: Tomato;"><strong>iterator</strong></span><span style="color: Tomato;">.</span>

  <strong>  1</strong><strong> │ </strong><span class="token variable">React</span><span class="token punctuation">.</span><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token keyword">function</span><span class="token punctuation">(</span><span class="token variable">x</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
  <strong><span style="color: Tomato;">&gt;</span></strong><strong> 2</strong><strong> │ </strong>  <span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
     <strong> │ </strong>         <span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span>
  <strong>  3</strong><strong> │ </strong><span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

  <strong><span style="color: DodgerBlue;">ℹ </span></strong><span style="color: DodgerBlue;">Keys help React identify which items have changed, are added, or are</span>
    <span style="color: DodgerBlue;">removed.</span>

</code></pre>{% endraw %}

---------------

{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token keyword">function</span><span class="token punctuation">(</span><span class="token variable">x</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text">
 <span style="text-decoration-style: dashed; text-decoration-line: underline;">file.tsx:2:8</span> <strong>lint/react/useKey</strong> ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  <strong><span style="color: Tomato;">✖ </span></strong><span style="color: Tomato;">Provide a </span><span style="color: Tomato;"><strong>key</strong></span><span style="color: Tomato;"> prop with a unique value for each element in </span><span style="color: Tomato;"><strong>iterator</strong></span><span style="color: Tomato;">.</span>

  <strong>  1</strong><strong> │ </strong><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token keyword">function</span><span class="token punctuation">(</span><span class="token variable">x</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
  <strong><span style="color: Tomato;">&gt;</span></strong><strong> 2</strong><strong> │ </strong>  <span class="token keyword">return</span> &lt;<span class="token attr-name">div</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
     <strong> │ </strong>         <span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span><span style="color: Tomato;"><strong>^</strong></span>
  <strong>  3</strong><strong> │ </strong><span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

  <strong><span style="color: DodgerBlue;">ℹ </span></strong><span style="color: DodgerBlue;">Keys help React identify which items have changed, are added, or are</span>
    <span style="color: DodgerBlue;">removed.</span>

</code></pre>{% endraw %}
### Valid
{% raw %}<pre class="language-text"><code class="language-text"><span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span>&lt;<span class="token attr-name">div</span> <span class="token attr-name">key</span><span class="token operator">=</span><span class="token string">&apos;a&apos;</span> <span class="token operator">/</span>&gt;<span class="token punctuation">,</span> &lt;<span class="token attr-name">div</span> <span class="token attr-name">key</span><span class="token operator">=</span><span class="token punctuation">{</span><span class="token string">&apos;b&apos;</span><span class="token punctuation">}</span> <span class="token operator">/</span>&gt;<span class="token punctuation">]</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text"><span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">x</span> <span class="token operator">=&gt;</span> &lt;<span class="token attr-name">div</span> <span class="token attr-name">key</span><span class="token operator">=</span><span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">)</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">React</span><span class="token punctuation">.</span><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> &lt;<span class="token attr-name">div</span> <span class="token attr-name">key</span><span class="token operator">=</span><span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">)</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> &lt;<span class="token attr-name">div</span> <span class="token attr-name">key</span><span class="token operator">=</span><span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">)</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text"><span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">x</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span> <span class="token attr-name">key</span><span class="token operator">=</span><span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">React</span><span class="token punctuation">.</span><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span> <span class="token attr-name">key</span><span class="token operator">=</span><span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token variable">x</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span> <span class="token attr-name">key</span><span class="token operator">=</span><span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text"><span class="token keyword">const</span> <span class="token variable">a</span> <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token keyword">function</span><span class="token punctuation">(</span><span class="token variable">x</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span> <span class="token attr-name">key</span><span class="token operator">=</span><span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">React</span><span class="token punctuation">.</span><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token keyword">function</span><span class="token punctuation">(</span><span class="token variable">x</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span> <span class="token attr-name">key</span><span class="token operator">=</span><span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
{% raw %}<pre class="language-text"><code class="language-text"><span class="token variable">Children</span><span class="token punctuation">.</span><span class="token variable">map</span><span class="token punctuation">(</span><span class="token variable">children</span><span class="token punctuation">,</span> <span class="token keyword">function</span><span class="token punctuation">(</span><span class="token variable">x</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">return</span> &lt;<span class="token attr-name">div</span> <span class="token attr-name">key</span><span class="token operator">=</span><span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&gt;<span class="token punctuation">{</span><span class="token variable">x</span><span class="token punctuation">}</span>&lt;<span class="token operator">/</span><span class="token attr-name">div</span>&gt;<span class="token punctuation">;</span>
<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span></code></pre>{% endraw %}
<!-- GENERATED:END(id:main) -->