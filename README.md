- 👋 Hi, I am Landa Shasi Kumar
- 👀 I’m interested in Data Science
      {{ with $person.education }}
      <div class="col-md-7">
        <h3>{{ i18n "education" | markdown }}</h3>
        <ul class="ul-edu fa-ul">
          {{ range .courses }}
          <li>
            <i class="fa-li fas fa-graduation-cap"></i>
            <div class="description">
              <p class="course">{{ .course }}{{ with .year }}, {{ . }}{{ end }}</p>
              <p class="institution">{{ .institution }}</p>
            </div>
          </li>
          {{ end }}
        </ul>
      </div>
      {{ end }

<!---
LSK30/LSK30 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
