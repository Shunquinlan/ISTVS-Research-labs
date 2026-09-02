# Data model and page structure

The directory is driven by one spreadsheet of lab records. Design the page
template and the spreadsheet columns together, and settle both **before** any
automation is written (that's the Week 4 task; the template is Week 3).

## Lab record fields

One row per research lab. Suggested columns — confirm with the maintainer and
the ISTVS Secretariat before treating as final, since the real dataset comes
from the retired Knack database:

| Field | Notes |
|---|---|
| `lab_name` | Display name of the laboratory |
| `institution` | University, company, or agency |
| `location` | City, State/Region, Country |
| `research_category` | One or more from a fixed category list (drives filtering) |
| `principal_investigator` | Name(s) |
| `description` | 1–3 sentence plain-language summary |
| `capabilities` | Research areas / equipment / facilities — short list |
| `website` | URL |
| `contact` | Email or contact page URL |
| `slug` | URL-safe id for the profile page filename (e.g. `iowa-state-terramechanics`) |

Keep the category list short and controlled (a handful of categories, not free
text) so filtering stays simple and consistent. Maintain the category list in
one obvious place.

## Pages

### Research Labs directory (landing page)

- Short intro: what this directory is and who it serves.
- Category navigation / filter — simple. A row of category links or buttons, or a
  single dropdown. Plain JavaScript filtering a static list is fine; no framework.
  If GitBook can't run the JS, fall back to one section per category.
- A grid of lab **cards** (see design system): name, institution, location, one
  line of description, link to the full profile.
- One clear call to action (e.g. "Submit a lab" / "Contact the Secretariat"),
  styled as the primary button.

### Lab profile page (reusable template)

One page per lab, generated from the template. Consistent structure for every lab:

- Heading: `lab_name`
- Institution · Location
- Description
- Capabilities / research areas (list)
- Principal investigator
- Website and contact links
- Back-to-directory link

Keep the template as plain Markdown with GitBook frontmatter so the automation
just fills in fields. Mark the fill points clearly (e.g. `{{lab_name}}`) in the
template file until the script exists.

## Placeholder records

Use these while designing and prototyping. Replace with the real dataset when
it's available. They are invented for layout purposes.

```csv
slug,lab_name,institution,location,research_category,principal_investigator,description,capabilities,website,contact
isu-terramechanics,Terramechanics & Soil-Machine Systems Lab,Iowa State University,"Ames, Iowa, USA",Soil-Vehicle Interaction,Dr. A. Researcher,"Studies tire and track performance on deformable soils using indoor soil bins and instrumented field vehicles.","Indoor soil bin; single-wheel tester; field data acquisition; DEM modeling",https://example.edu/terramechanics,labs@example.edu
mtu-winter-mobility,Winter Mobility Research Group,Michigan Technological University,"Houghton, Michigan, USA",Snow & Ice Mobility,Dr. B. Investigator,"Evaluates vehicle mobility on snow and ice, including tire traction and thermal effects.","Cold-room test track; snow characterization; traction dynamometer",https://example.edu/winter-mobility,winter@example.edu
army-erdc-mobility,Mobility Systems Branch,US Army ERDC,"Vicksburg, Mississippi, USA",Off-Road Vehicle Performance,Dr. C. Scientist,"Federal laboratory researching off-road vehicle performance and terrain modeling for defense applications.","Mobility modeling; large-scale soil bins; terrain mapping; NRMM/NG-NRMM",https://example.gov/mobility,mobility@example.gov
tu-berlin-offroad,Off-Road Vehicle Dynamics Lab,Technical University of Berlin,"Berlin, Germany",Vehicle Dynamics,Dr. D. Forscher,"Investigates off-road vehicle dynamics and driver-assistance systems for agricultural machinery.","Multibody simulation; test tractor fleet; soil-tire test rig",https://example.de/offroad,offroad@example.de
```
