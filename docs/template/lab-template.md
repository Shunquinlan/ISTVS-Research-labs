---
description: "{{short_description}}"
---

<!--
  ISTVS Research Labs – LAB PAGE TEMPLATE (DRAFT, not approved yet)

  How to use:
  - Each {{field_name}} is filled from the matching column in the lab spreadsheet.
  - If a field is empty for a lab, delete that whole line or section
    (heading included). Never publish a heading with nothing under it.
  - Sections marked OPTIONAL only appear when the lab has that information.
  - This comment block is not shown on the website.
-->

# {{lab_name}}

<figure><img src="{{logo_url}}" alt="{{lab_name}} logo" width="200"><figcaption></figcaption></figure>

| Lab details      |                                              |
| ---------------- | -------------------------------------------- |
| Institution      | {{institution}}                              |
| Location         | {{city}}, {{state_region}}, {{country}}      |
| Type             | {{lab_type}}                                 |
| Research areas   | {{research_areas}}                           |
| Lab lead         | {{pi_name}}                                  |
| Open to          | {{open_to}}                                  |

<a href="{{website}}" class="button primary">Visit the lab website</a> <a href="mailto:{{contact_email}}" class="button secondary">Email the lab</a>

## Overview

{{overview}}

## Facilities and equipment

{{facilities_equipment}}

<!-- OPTIONAL: only when the lab has photos -->
<figure><img src="{{photo_1_url}}" alt="{{lab_name}} – facility photo"><figcaption></figcaption></figure>

<!-- OPTIONAL -->
## Soils and test materials

{{soils_available}}

Other options: {{soil_options}}

<!-- OPTIONAL -->
## Services for external partners

{{services}}

<!-- OPTIONAL -->
## Selected research and publications

{{research_projects}}

<!-- OPTIONAL -->
## Highlights

{{highlights}}

## Contact

{{pi_name}}
{{director_name}}
[{{contact_email}}](mailto:{{contact_email}})

<!-- OPTIONAL: only when the lab has a brochure -->
[Download the lab brochure (PDF)]({{brochure_url}})

{% hint style="info" %}
Information provided by the laboratory and last reviewed on {{last_reviewed}}. To update this listing, contact the ISTVS General Secretariat.
{% endhint %}

[← Back to all research labs](../README.md)
