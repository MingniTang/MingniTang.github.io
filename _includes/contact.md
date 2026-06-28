<h1 id="contact"></h1>

<h2 style="margin: 60px 0px 10px;">Contact</h2>

<p>
{% if site.email %}
<strong>Email:</strong> <email>{{ site.email }}</email>
{% endif %}
{% if site.email2 %}
<br />
<strong>Alternative email:</strong> <email>{{ site.email2 }}</email>
{% endif %}
{% if site.email3 %}
<br />
<strong>Alternative email:</strong> <email>{{ site.email3 }}</email>
{% endif %}
</p>
