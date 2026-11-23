# What is the Met missing? 
### _A data-driven approach to identifying underrepresented and underdocumented cultures in the Met's collection_

## Summary
[Write last: the finding for the head of collections, in 3-4 sentences.]

## Business Problem
The museum wants to know where to focus cataloguing resources and which types of artifact
(era, find-spot information) to research through partnerships or loans from other museums, since cataloguing resources are finite and loans are limited.  
To support this decision we establish different time bands and ask for each one of these: which cultures are underrepresented or underdocumented in the catalogue?

- **Presence:** which cultures have a small share of the collection within each time band?
- **Documentation:** which cultures' objects sit in the lower documentation tiers within each time band?  

The decision of using time windows is based on the fact that cultures flourished at very different times and places, so one shared timeline would misrepresent them.

By underrepresented we mean that the culture has a small share of the collection within a time band, specifically, an amount in the bottom quartile of its group. By underdocumented we mean that the objects from that culture are in the lower documentation tiers for time and place information.

**Stakeholder:** head of collections.  
**Decision supported:** what to focus research efforts on.

## Methodology
1. **Data:** All raw data is contained in the file MetObjects.txt, taken from the Met's Open Access dataset (CC0) on 21/11/2026.
2. **Scope:** 4500 BCE to 1500 CE. The time bands are nameless in order to avoid imposing any ideology onto them; the three time bands are 4500–1000 BCE, 1000 BCE–500 CE and 500–1500 CE. Objects dated in a range that overlaps two bands are assigned to the band with the larger overlap.
3. **Culture groups:** Cultural subgroups are merged under "parent" cultures using a mapping table;
   cultural groups that present under 10 objects in a certain time band are merged into "Other"; objects with no recorded culture are inserted under "Culture not recorded".
4. **Presence:** [your measure, within each band].
5. **Documentation tiers:** Objects will be classified using a tier system for both time and place/maker information. The tiers are defined as follows:  
   - Time: tier 1 is the precise year or a 25-year range, tier 2 is knowing the century or a 100-year range, tier 3 is knowing an approximate century or era, with a range larger than 200 years. Where applicable, having information on the dynasty is considered  tier 2 and having information on the reign is considered tier 1.
   - Place: tier 1 is the precise city or even artisan workshop or name, tier 2 is the region, tier 3 is country (modern political borders corresponding to where the artifact was found).  

The lowest tier is "no information" for both time and place. Placeholder text such as "Unknown" or "date uncertain" are counted as missing.
6. **Comparison (Python):** [how you compare groups, and minimum group size].
7. **Dashboard:** [Power BI].

## Skills
[Later.]

## Results & Business Recommendation
[Presence findings.] [Documentation findings.] [Recommendation: where to focus cataloguing; which eras/regions to pursue for partnerships.]
**Limitations:** [Collecting history of one museum; no external benchmark; culture labels are curatorial constructs; no provenance column; tier cutoffs are our choices.]