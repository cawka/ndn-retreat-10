---
layout: default
title: Accommodations
group: Local Information

hotels:
- category: Closest
  expanded: True
  hotels:
  - id: holiday
    name: Holiday Inn at U. Memphis
    rates: $120+
    amenities: []
    address: 
    url: "https://www.ihg.com/holidayinn/hotels/us/en/memphis/memkw/hoteldetail"
    phone: 901-678-8200
    reservation-link: "https://www.ihg.com/holidayinn/hotels/us/en/find-hotels/hotel/rooms?qDest=3700%20Central%20Avenue,%20Memphis,%20TN,%20US&qCiMy=22022&qCiD=24&qCoMy=22022&qCoD=27&qAdlt=1&qChld=0&qRms=1&qRtP=6CBARC&qSlH=MEMKW&qAkamaiCC=US&qSrt=sBR&qBrs=re.ic.in.vn.cp.vx.hi.ex.rs.cv.sb.cw.ma.ul.ki.va.ii.sp.nd.ct.sx.we.lx&qAAR=6CBARC&qWch=0&qSmP=1&setPMCookies=true&qRad=30&qRdU=mi&srb_u=1&qpMn=0&qSHBrC=HI"

---

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
