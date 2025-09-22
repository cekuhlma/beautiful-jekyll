---
layout: page
---

<div class="post">
  <header>
    <h1>{{ page.title }}</h1>
  </header>

  <table class="ryan-table">
    <thead>
      <tr>
        <th>Ryan Reynolds</th>
        <th>Ryan Gosling</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
          <strong>Strengths</strong>
          <ul>
            {% for s in page.reynolds.strengths %}
              <li>{{ s }}</li>
            {% endfor %}
          </ul>
          <strong>Weaknesses</strong>
          <ul>
            {% for w in page.reynolds.weaknesses %}
              <li>{{ w }}</li>
            {% endfor %}
          </ul>
        </td>
        <td>
          <strong>Strengths</strong>
          <ul>
            {% for s in page.gosling.strengths %}
              <li>{{ s }}</li>
            {% endfor %}
          </ul>
          <strong>Weaknesses</strong>
          <ul>
            {% for w in page.gosling.weaknesses %}
              <li>{{ w }}</li>
            {% endfor %}
          </ul>
        </td>
      </tr>
    </tbody>
  </table>

  <div class="content">
    {{ content }}
  </div>
</div>

<style>
.ryan-table { border-collapse: collapse; width: 100%; margin: 1rem 0; }
.ryan-table th, .ryan-table td { border: 1px solid #ddd; padding: 10px; vertical-align: top; }
.ryan-table thead th { background: #f5f5f5; text-align: left; }
</style>
