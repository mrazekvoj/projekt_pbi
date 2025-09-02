# Israeli legislative elections (2009–2015)

Interactive report about Israeli Knesset elections (2009, 2013, 2015): party results, custom party **categories**, and maps by **winning party** or **district averages**.

**Live report (public):** [Open in Power BI service](https://app.powerbi.com/view?r=eyJrIjoiOTQ3OGYyYWQtNjY2Yi00MTg5LTg0OGYtOWZlZjk0MzdiOTFlIiwidCI6ImM4ZjhlZDkxLWUzZmYtNGI2Yi1iZjJjLTczNjBmNWNlNDY1OCIsImMiOjl9)

---

## How to use the report
- **Select an election year** (2009/2013/2015).  
- **Complete results** – vote share by party.  
- **Map of localities by winning party** – dots colored by the party that won each locality.  
- **District table & map** – average vote share by **party category** per district.  
- **Search / filters** – full-text locality search, optional West Bank-only toggle.  
- **Cards** – show selected locality, winning party and its category.
 
---

## Party categories (used in the visuals)
- **Arab parties** – Sum of vote shares for parties elected mostly by Arab citizens of Israel, with Arab-led lists.  
- **Far Right** – Parties including ultranationalism; in some cases currents associated with Jewish supremacy/fascism and explicit anti-Arab positions.  
- **Left–center** – Sum of left and centrist parties that positioned themselves against right/Haredi/Religious-Zionist blocs.  
- **Ultraorthodox** – Parties representing Ashkenazi and Sephardi Haredim (e.g., United Torah Judaism, Shas).  
- **Likud & Yisrael Beiteinu** – Combined vote of Likud and the secular-nationalist Yisrael Beiteinu (joint or separate lists).  
- **Religious Zionism** – Right-wing Religious-Zionist parties; typically support settlement in Judea & Samaria / the West Bank.  
- **Others** – Minor or unaffiliated lists.

*(Each party is mapped to exactly one category per election year.)*

---

## Notes
- Map visuals use **Shape map** (districts, TopoJSON) and/or **custom Icon Map** (locality dots) so the report works even when Bing Maps visuals are disabled in a tenant.  
- Colors for parties are defined directly in the model (`parties[color_hex]`) for consistency across visuals.  
- “Winning party” logic: for the current locality & year, the party with the highest `party_votes_share` is shown; the map draws only winning dots.
