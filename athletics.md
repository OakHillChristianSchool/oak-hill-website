---
layout: simple-title-formatted
title: Athletics
---

<div uk-grid>
  <div class="uk-width-2-3@m">
    <p>Oak Hill Christian Schools encourages students to sign up for sport with the Chantilly Youth Association (CYA).</p>
    <p>CYA offers recreational and travel leagues for a variety of sports. We are excited to have our students be part of this league and encourage our students to sign up for soccer, basketball (winter), football, baseball and volleyball. CYA will make an effort to place friends on the same team but make sure to write their name down during registration.</p>
    <p>Sign up early for registration discounts.</p>
    <p>If you have any questions, please contact our athletics director, <a href="mailto:agil@oakhillk12.com">Arelis Gil</a>.</p>
  </div>
  <div class="uk-width-1-3@m">
    <img src="assets/cya-logo.png" alt="CYA logo">
  </div>
</div>

<table class="uk-table uk-table-striped">
  <thead>
    <tr>
      <th>Sport</th>
      <th>Program Fee</th>
      <th>Details</th>
    </tr>
  </thead>
  <tbody>
    {% for sport in site.data.athletics.sports %}
    <tr>
      <td>{{ sport.title }}</td>
      <td>{{ sport.fee }}</td>
      <td><a href="{{ sport.details_link }}" target="_blank">Details</a></td>
    </tr>
    {% endfor %}
  </tbody>
</table>

<p>Prices may vary for travel teams.</p>
