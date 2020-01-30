---
layout: default
title: Accommodations
group: Local Information

hotels:
- category: On Campus
  expanded: True
  hotels:
  - id: tbd
    name: Name
    rates: $000+
    amenities: []
    address: 
    url: 
    phone: 
    reservation-link: https://luskinconferencecenter.ucla.edu/reserve/
    note: "."

---

{% comment %}
map: "https://www.google.com/maps/embed?pb=!1m28!1m12!1m3!1d3305.0031903347244!2d-118.44719493474814!3d34.06943247427142!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!4m13!3e2!4m5!1s0x80c2bc8602a90341%3A0xd73874d4f138751a!2sUCLA+Meyer+and+Renee+Luskin+Conference+Center%2C+Westwood+Plaza%2C+Los+Angeles%2C+CA!3m2!1d34.069179!2d-118.445718!4m5!1s0x80c2bc88bcefb20f%3A0xc622b89fcd2f5d21!2sEngineering+VI%2C+Westwood+Plaza%2C+Los+Angeles%2C+CA+90095!3m2!1d34.0696771!2d-118.4442945!5e0!3m2!1sen!2sus!4v1522597689735"
{% endcomment %}

# {{ page.title }}

We have compiled this list to assist you in arranging accommodations.

**Please keep in mind that the listed prices are subject to change daily and/or seasonally**

{% for hotels in page.hotels %}

## {{ hotels.category }}

<div class="panel-group" id="accordion">
{% for hotel in hotels.hotels %}
{% include hotel.html expanded=hotels.expanded %}
{% endfor %}
</div>
---
{% endfor %}
