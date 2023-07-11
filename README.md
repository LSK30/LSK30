- 👋 Hi, I am Landa Shasi Kumar
- 👀 I’m interested in Data Science
  {{ with $person.education }}
      <div class="col-md-7">
        <h3>{{ i18n "education" | markdown }}</h3>
        <ul class="ul-edu fa-ul">
          {{ range .courses }}
          <li>
            <!--https://github.com/catrincm/personal-website/blob/e06b3525f51a3dd2653578a29c9b5b253596ab1a/layouts/partials/widgets/about.html-->
            {{ if .course }}
            <i class="fa-li fas fa-graduation-cap"></i>
            <div class="description">
              <p class="course">{{ .course }}{{ with .year }}, {{ . }}{{ end }}</p>
              <p class="institution">{{ .institution | markdown }}</p>
              <!--https://github.com/gcushen/hugo-academic/issues/1094#issuecomment-622200594-->
            </div>
            {{ end }}
            {{ if .certificate }}
            <i class="fa-li fas fa-certificate"></i>
            <div class="description">
              <p class="course">{{ .certificate }}{{ with .year }}, {{ . }}{{ end }}</p>
              <p class="institution">{{ .institution | markdown }}</p>
              <!--https://github.com/gcushen/hugo-academic/pull/951#issue-255104712-->
            </div>
            {{ end }}

          </li>
          {{ end }}
        </ul>
      </div>
      {{ end }}

<!---
LSK30/LSK30 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
