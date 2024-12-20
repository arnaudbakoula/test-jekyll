<article id="{{ include.id }}">
  <h2 class="major">{{ include.id | capitalize }}</h2>
  <form method="post" action="#">
    <div class="fields">
      {% for field in site.data.contact.form.fields %}
      <div class="field">
        <label for="{{ field.name | downcase }}">{{ field.label }}</label>
        {% if field.type == "textarea" %}
        <textarea
            name="{{ field.name | downcase }}"
            id="{{ field.name | downcase }}"
            rows="4"
            placeholder="{{ field.placeholder }}"
            required="{{ field.required }}"></textarea>
        {% elsif field.type == "select" %}
        <select
            name="{{ field.name | downcase }}"
            id="{{ field.name | downcase }}">
          <option value="">-</option>
          {% for option in field.options %}
          <option value="{{ option }}">{{ option }}</option>
          {% endfor %}
        </select>
        {% else %}
        <input
            type="{{ field.type }}"
            name="{{ field.name | downcase }}"
            id="{{ field.name | downcase }}"
            placeholder="{{ field.placeholder }}" />
        {% endif %}
      </div>
      {% endfor %}
    </div>
    <ul class="actions">
    {% for action in site.data.contact.form.actions %}
      <li><input type="{{ action.type }}" value="{{ action.value }}" class="{{ action.primary }}" /></li>
    {% endfor %}
    </ul>
  </form>
</article>
