---
layout: advisors
title: "Current & previous advisors"
---

{{ content }}

<h3 class="fw-bold border-bottom pb-3 mb-5">Current & Previous  Advisors </h3>
{% for person in site.data.settings.advisors %}
<div class="row g-5 mb-5">
  <div class="col-md-6">
    <h5>{{ person.name }}</h5>
    <p>Email: {{ person.email }}</p>
    <p>Title: {{ person.title }}</p>
    <p>Department: {{ person.department }}</p>
    <p>Institution: {{ person.institution }}</p>
    <p>Institution address: {{ person.institution_address }}</p>
    <p>Email: {{ person.email }}</p>
    <p><a href="{{ person.url }}">Related Websites</a></p>
  </div>
  <div class="col-md-6">
    <img src="/{{ person.image }}" alt="Contact" width="50%">
  </div>
</div>
{% endfor %}

advisors:
- {name: 'Colin Kinz-Thompson', title: 'Assistant Professor', department: 'School of Arts & Sciences-Newark', institution: 'Rutgers, The State University of New Jersey', institution_address: 'Olson Hall, 73 Warren St, Rutgers University-Newark, Newark, NJ 07102', email: 'colin.kinzthompson@rutgers.edu', image: 'assets/img/colin.jpg', url: 'https://ckinzthompson.github.io'}
- {name: 'Guangfeng Wang', title: 'Assistant Professor', department: 'School of Chemistry and Materials Science', institution: 'Anhui Normal University | AHNU', institution_address: 'Wuhu, Anhui, China', email: 'wangyuz@mail.ahnu.edu.cn', image: 'assets/img/wangguangfeng.jpg', url: 'https://www.researchgate.net/profile/Guangfeng-Wang-2'}
