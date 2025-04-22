---
title: "Subscriber"
draft: false
description: "Testing subscriber form"
layout: newsletter
---
<form
  action="https://buttondown.com/api/emails/embed-subscribe/NaturCeredigion"
  method="post"
  target="popupwindow"
  onsubmit="window.open('https://buttondown.com/NaturCeredigion', 'popupwindow')"
  class="embeddable-buttondown-form"
>
  <label for="bd-email">Enter your email</label>
  <input type="email" name="email" id="bd-email" />
  <label for="family_name">Family name</label>
  <input type="text" name="metadata__family_name" id="family_name" />
  <label for="member_details">Organisation</label>
  <input type="text" name="metadata__organisation" id="organisation" />
  <label for="given_name">Given name</label>
  <input type="text" name="metadata__given_name" id="given_name" />
  <label for="org">org</label>
  <input type="text" name="metadata__org" id="org" />
  <label for="member">member</label>
  <input type="text" name="metadata__member" id="member" />
  <label for="Subscribe">Subscribe</label>
  <input type="submit" value="Subscribe" />
  <p>
    <a href="https://buttondown.com/refer/NaturCeredigion" target="_blank">Powered by Buttondown.</a>
  </p>
</form>
