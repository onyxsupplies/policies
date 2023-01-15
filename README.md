# Datica HIPAA Compliance Policies

## A quick note from Onyx

The original repository from Datica, along with its other websites and domains are no longer online, but I am retaining its references where appropriate for crediting.

—Ian Mckenzie, Onyx's MVP developer

## Introduction

HIPAA compliance is complicated, but it doesn't have to be. Datica helps relieve the technical burden with our HIPAA-compliant cloud computing platform and solutions for healthcare.

In an effort to make compliance as easy as possible for companies working with protected health information (PHI), we decided to open source our company policies.

Our policies have been written with modern, cloud-based technology vendors in mind. We looked far and wide for policy examples that fit our company, and couldn't find any. So we wrote our own. Importantly, these policies have been through three external audits—two HIPAA audits and one HITRUST audit.

Do you handle PHI and not yet have your own company policies in place? Then you'll find our content useful.

## Why did we open source these policies?

HIPAA compliance really has two halves. The first half includes all technical guidelines, both physical and digital. Compliant companies take measures to secure their hardware and manage their software in a certain way. Encryption, logging, monitoring—these are just a few examples of HIPAA technical requirements. Datica builds its platform with these guidelines in mind.

The second half of HIPAA is focused on administrative and organizational activities. This includes signing Business Associate Agreements (BAAs), and managing company policies like training, among other things. Crafting company policies that align with HIPAA administrative guidelines are straightforward, but an immense burden.

When we were creating our policies, we found lots of policy templates for healthcare providers, but nothing for modern health technology companies. We spent a lot of time and effort writing our policies, then adapting them to meet the demands of external audits. We don't want people to reinvent the wheel; trust us, it's not fun. We also feel a broader community can improve these polices over time, making them better for everybody.

By open sourcing our own company policies, we hope other companies who handle PHI will benefit. It aligns with our company mission: to help you focus on building innovative healthcare applications.

## What do I do with these policies?

As a company who handles PHI, it's critical you maintain and publish your own policies. To make use of our policies, we recommend the following steps.

1. Read through all the enclosed policies to get an understanding to the structure.
2. When ready, download the policies and comb through for mentions of Datica or our business and change to appropriate references to your company.
3. Publish your policies in a publicly available location. The files are markdown, so you may need to convert to HTML if you don't have a publishing platform capable of markdown format. You can either create an index page linking to each individual policy, or create a single page listing all the policies in line, [much like we did](https://policy.datica.com).

## Who is behind this?

[Datica](htts://datica.com), healthcare's trusted HITRUST CSF Certified digital health platform.

We help companies who handle PHI, both business associates and covered entities, maintain compliance with our ([Compliant Cloud](https://datica.com/compliant-cloud)) and ([Managed Integration](https://datica.com)).

To get in touch, shoot us an email at [hello@datica.com](mailto:hello@datica.com). We'd love to hear from you!

### License

All policies are licensed under [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/).

### Policy Index

Each policy is included as its own markdown file in case you want to cherry-pick specific policies. If you currently have no policies in place, we encourage you to consider utilizing all compliance policies.

* [Introduction](source/sections/01-introduction.md)
* [HIPAA Inheritance](source/sections/02-hipaa_inheritance.md)
* [Policy Management Policy](source/sections/03-policy_management_policy.md)
* [Risk Management Policy](source/sections/04-risk_management_policy.md)
* [Roles Policy](source/sections/05-roles_policy.md)
* [Data Management Policy](source/sections/06-data_management_policy.md)
* [System Access Policy](source/sections/07-systems_access_policy.md)
* [Auditing Policy](source/sections/08-auditing_policy.md)
* [Configuration Management Policy](source/sections/09-configuration_management_policy.md)
* [Facility Access Policy](source/sections/10-facility_access_policy.md)
* [Incident Response Policy](source/sections/11-incident_response_policy.md)
* [Breach Policy](source/sections/12-breach_policy.md)
* [Disaster Recovery Policy](source/sections/13-disaster_recovery_policy.md)
* [Disposable Media Policy](source/sections/14-disposable_media_policy.md)
* [IDS Policy](source/sections/15-ids_policy.md)
* [Vulnerability Scanning Policy](source/sections/16-vulnerability_scanning_policy.md)
* [Data Integrity Policy](source/sections/17-data_integrity_policy.md)
* [Data Retention Policy](source/sections/18-data_retention_policy.md)
* [Employees Policy](source/sections/19-employees_policy.md)
* [Approved Tools Policy](source/sections/20-approved_tools_policy.md)
* [3rd Party Policy](source/sections/21-3rd_party_policy.md)
* [Key Definitions](source/sections/22-key_definitions.md)
* [Onyx HIPAA Business Associate Agreement (“BAA”)](source/sections/23-onyx_hipaa_business_associate_agreement.md)
* [HIPAA Mappings to Onyx Controls](source/sections/24-hipaa_mapping_to_onyx_controls.md)

### How to build the docs

- Download this repository
  * Option one (https): `git clone https://github.com/onyxsupplies/policies`
  * Option two (ssh): `git@github.com:wettowelreactor/policies.git`
  * Option three (zip): Download the zip file from [https://github.com/onyxsupplies/policies](https://github.com/onyxsupplies/policies)
  * Option four (à la carte): Your preferred method of downloading from GitHub: `onyxsupplies/policies`
- `cd policies`
- `gem install bundler --version=2.0.1`
- `bundle install`

*Commands*
- `rake run` will run the site locally
- `rake sass` will compile any changes made to `assets/css/styles.scss`
- `rake build` will build the static site into the `build` directory
- `rake serve_static` will create a simple HTTP server for the `build` directory