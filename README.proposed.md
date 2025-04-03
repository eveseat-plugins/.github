# The EveSeat Plugin Organisation

## The Rationale

The SeAT Plugin Organisation is a collaborative community-driven initiative designed to support the ongoing maintenance and development of SeAT plugins. The core goal is to empower plugin owners to independently manage their plugins, while offering a safety net in cases where the primary maintainers are unavailable. The organisation’s leadership team is available to step in in during critical situations such as patching urgent vulnerabilities or updating plugins to new SeAT versions in the absence of the primary maintainer, ensuring continuity and stability for the community.

Plugins that are actively maintained, open-sourced, and useful to others can opt into the organisation. In cases where a plugin is considered essential but its maintainer is inactive, the organisation may fork the plugin to ensure its continued support. This will only happen after making an attempt to contact the original developer. Forked plugins will have a new primary maintainer, but the original developer is welcome to return and reclaim ownership if they become active again.

### Level of Support

This organisation is not a space for free-for-all feature development; plugin feature development remains the responsibility of the plugin owners themselves.

Being part of the SeAT Plugin Organisation does not guarantee that patches or updates will be made to a plugin. While the organisation offers a support structure where the leadership team can step in to address critical issues, such as security vulnerabilities or compatibility updates, these actions are not automatic. However, by joining the organisation, plugin owners increase the likelihood that their plugins will receive attention in the event of urgent circumstances or when they are unavailable to maintain them. This makes the possibility of timely patches more feasible, but it is not a promise that every plugin will always be maintained or updated by the organisation.

By default, the leadership team only expects to step in to merge / maintain code if the primary maintainer is inactive and unresponsive. In the outset the timelines for inactivity will be handled on a case by case basis with a typical critical PR being considered as inactive if no response is received in a month. Note that a critical PR would be for a security fix, or fix for broken functionality due to a SeAT update. Feature PRs are not critical.

## Requirements

There are very few requirements in order for a plugin to be accepted into the organisation, as it is intentionally a goal to be as welcoming as possible.

### License

The plugin must be open source with a license that is compatible with the GPLv2 (as SeAT is licensed under GPLv2 and plugins are considered single combined programs).

### Utility

The plugin should be something that is useful to other users of seat, not something that will only function for you or your group. ie a plugin that has counter espionage functionality that works within data that is either wholly contained in SeAT, or works with other tools that are widely available is fine. A counter intelligence tool that links into non-available tools that are private to your organisation is not considered useful to others. ie, please don't try and add `seat-private-internal-goon-intel-tool` into the org.

### Packagist

The plugin should be published on packagist (and updated to ensure it points at the org once the plugin is moved). This is what allows the eve plugins to be so easily added by users and as such is considered mandatory. Packagist should be configured to update automatically when github releases are tagged.

#### composer.json

This is the file used by composer to detail relevant information about your package. It is expected that this is kept up to date, including the authors section.
In the future this file will also be parsed to populate plugin information on this page.

## Contact
Whether you want to start a new plugin in this organization, transfer an already existing one, or take over the maintenance of an abandoned plugin, please feel free to contact `@recursive_tree` or `@crypta_electrica` on the [SeAT Discord](https://discord.gg/VcUZRcnMYK).