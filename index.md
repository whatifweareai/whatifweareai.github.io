---
layout: default
---
<section class="hero">
  <div class="hero-text">
    <h1>{{ site.title }}</h1>
    <p class="subtitle">{{ site.subtitle }}</p>
    <p class="tagline"><em>{{ site.tagline }}</em></p>
    <p class="byline">by {{ site.author }}</p>
    <p class="buy"><span>Get the Kindle ebook ({{ site.price_note }}):</span>
      {% for link in site.buy_links %}<a class="store" href="{{ link.url }}">{{ link.label }}</a>
      {% endfor %}
    </p>
    <p class="inside-link"><a href="{{ '/inside/' | relative_url }}">See the contents and read six passages</a></p>
  </div>
  <div class="book">
    <span class="hum" aria-hidden="true"></span>
    <img src="{{ '/assets/img/cover.jpg' | relative_url }}" width="562" height="900" fetchpriority="high" alt="Cover of {{ site.title }}: {{ site.subtitle }}">
  </div>
</section>

When I was a boy, a computer read eight digits of my birth data and made two predictions about my life. Both came true.

That evening has bothered me ever since. If a machine can call a life in advance, then a life is the kind of thing that can be called in advance, and that is a far stranger fact than any horoscope.

*The Hum* is a memoir and an argument. Years later, while training convolutional neural networks, I began to notice that the words of training (weights, gradients, dropout, a run with a purpose) described my own life uncomfortably well. So the book asks: what if we are not the programmers but the model?

It does not ask you to believe. The first page says it is a work of fiction, until science proves it to be the truth.

Read it as an argument you are free to lose. Read it as the story of a mother who came home happy. Either way, the destination is not proof. It is peace.

<section class="subscribe" aria-labelledby="subscribe-heading">
<h2 id="subscribe-heading">Notes from the author</h2>
<p>Occasional updates about the book. No spam, and you can unsubscribe at any time.</p>
<form action="https://buttondown.com/api/emails/embed-subscribe/whatifweareai" method="post" target="_blank">
<label for="subscribe-email">Your email address</label>
<div class="subscribe-row">
<input type="email" name="email" id="subscribe-email" required autocomplete="email">
<input type="submit" value="Subscribe">
</div>
</form>
<p class="credit"><a href="https://buttondown.com/refer/whatifweareai">Powered by Buttondown</a></p>
</section>

*For Amma, who came home happy, and Achan who walked with me.*
