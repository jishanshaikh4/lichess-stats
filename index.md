<ul>
{% for member in site.data.lichess-stats %}
  <li>
    <a href="https://lichess.org/@/{{ member.username }}">
      {{ member.username }}
    </a>
    
    <a href="https://lichess.org/@/{{ member.username }}">
      {{ member.bullet.rating }}
    </a>
  </li>
{% endfor %}
</ul>
