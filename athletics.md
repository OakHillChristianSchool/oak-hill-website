---
layout: simple-title-formatted
title: Athletics

---
<div uk-grid> <div class="uk-width-2-3@m"> <p>Oak Hill Christian School has teamed up with i9 Sports! i9 Sports will try to ensure that you and your Oak Hill friends are on the same team, but in order for that to happen you must enter your friend's name during registration when prompted.</p> <p>Play a sport with your friends! i9 Sports offers co-ed teams for various sports.</p> </div> <div class="uk-width-1-3@m"> <img src="assets/i9-logo.png" alt="i9-sports logo"> </div> </div>

<h3>Registration now open for the fall! (Locations may vary)</h3>

<table class="uk-table uk-table-striped">
<thead>
<tr>
<th>Sport</th>
<th>Start Date</th>
<th>End Date</th>
<th>Grades</th>
<th>Program Fee</th>
<th>Details</th>
</tr>
</thead>
<tbody>
{% for sport in site.data.athletics.sports %}
<tr>
<td>{{ sport.title }}</td>
<td>{{ sport.start_date }}</td>
<td>{{ sport.end_date }}</td>
<td>{{ sport.grades }}</td>
<td>{{ sport.fee }}</td>
<td><a href="{{ sport.details_link }}" target="_blank">Details</a></td>
</tr>
{% endfor %}
</tbody>
</table>