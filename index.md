---
layout: page
title:
subtitle:
---

{% raw %}
<style>
/* Jekyll 기본 타이틀 숨김 */
.page-title,
.page-subtitle { display: none !important; }

/* 페이지 전체 폭 — 필요시 1800~2000px로 조절 */
.page-content, .container {
  max-width: 1800px !important;
  margin: auto;
  padding-left: 30px;
  padding-right: 30px;
}

/* ====== 소개 섹션 (항상 좌:이미지 / 우:텍스트) ====== */
.intro-container {
  /* 데스크톱에서는 2열 고정 */
  display: grid;
  grid-template-columns: clamp(260px, 20vw, 360px) 1fr; /* 왼쪽 고정폭, 오른쪽 유동 */
  column-gap: 48px;
  align-items: start;
  margin-bottom: 2rem;
}

.intro-img-wrapper { 
  /* 그리드 1열: 이미지 칼럼 */
  width: 100%;
}
.intro-img-wrapper img {
  width: 100%;
  height: auto;
  border-radius: 12px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  display: block;
}

.intro-text {
  /* 그리드 2열: 텍스트 칼럼 */
  font-size: 1.1rem;
  line-height: 1.8;
  /* 너무 좁아지지 않게 최소 폭 확보 */
  min-width: 700px;                 /* ★ 텍스트 가로폭 확보 포인트 */
  /* 단어 줄바꿈 이슈 대비 */
  word-break: keep-all;
  overflow-wrap: anywhere;
}

/* 브라우저가 아주 넓을 때 텍스트 칼럼이 너무 길어지면 읽기 어려우니 최대 폭 제한을 주고 싶다면 아래 주석 해제
.intro-text { max-width: 95ch; }
*/

/* ====== 반응형: 태블릿/모바일에서만 세로 스택 ====== */
@media (max-width: 1100px) {
  .intro-container {
    grid-template-columns: clamp(220px, 28vw, 300px) 1fr;
    column-gap: 36px;
  }
  .intro-text { min-width: 0; }  /* 좁은 화면에서는 제한 해제 */
}

@media (max-width: 780px) {
  .intro-container {
    display: block;   /* 모바일에서만 위/아래 스택 */
  }
  .intro-img-wrapper { margin-bottom: 20px; max-width: 420px; }
}
</style>
{% endraw %}

<div class="intro-container">
  <div class="intro-img-wrapper">
    <img src="/assets/img/headshot_jongwoo.jpeg" alt="Jongwoo Jeong">
  </div>
  <div class="intro-text">
    <p>Hi everyone — it’s great to e-meet you!</p>

    <p>I'm Jongwoo Jeong, an Assistant Professor of Political Science at 
    <a href="https://politicalscience.gsu.edu/">Georgia State University</a>.</p>

    <p>I earned my Ph.D. from Texas A&M University in 2022 and completed a two-year postdoctoral fellowship at Washington University in St. Louis. My research examines how polarization and immigration shape American political life across native-born and immigrant populations, with particular attention to political participation, political incorporation, and representation. While grounded in political behavior, my work also integrates perspectives from institutional analysis, public administration, and the politics of crime and criminal justice. Methodologically, I employ a broad set of approaches, including text-as-data, experimental design, causal inference, geographical and geo-political analyses, as well as computational social science (e.g., machine learning and generative AI) for political research. Through this approach, I study how democracy in the United States evolves and endures across diverse populations, institutions, and political contexts.</p>

    <p>My work has been published or is forthcoming in journals such as <em>American Journal of Political Science</em>, <em>Journal of Politics</em>, <em>British Journal of Political Science</em>, and <em>Political Behavior</em>, as well as in outlets focused on race and ethnicity like <em>Politics, Groups, and Identities</em>. I've been fortunate to receive support from the APSA Centennial Center and the APSA Advancing Research Grant for Early Career Scholars. For more details, you can <a href="/assets/img/cv_aug.pdf" target="_blank">view my CV here </a>.</p>

    <p>I’m always excited to connect, collaborate, and learn from others—so feel free to reach out!</p>
  </div>
</div>

---

## Contact






```
Affiliation: Department of Political Science, Georgia State University
Mailing Address: Georgia State University, Department of Political Science, 38 Peachtree Center Ave SE, Room 1023, Atlanta, GA 30303
Email: jjeong15[at]gsu.edu
```
