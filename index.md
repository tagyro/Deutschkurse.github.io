<html>
<head>
</head>
<body>
   <ul>
        {% for post in paginator.posts %}
        <li>
          <p>
            <a href="{{ site.baseurl}}{{ post.url }}"> {{ post.title }}</a><br />
          {{ post.date | date: "%b %-d, %Y" }}
          </p>
        </li>
        {% endfor %}
      </ul>
</body>
</html>
