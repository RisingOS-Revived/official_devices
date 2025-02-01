# Rising OS Maintainers Code of Conduct

**Note:** This document will always be updated from time to time. Check regulary to make sure you are caught up on any updates.

Levels of Punishment if the particular rule is broken.
- **L0 class:** This is just here to make sure you read actually read the important information as well. Failure to do so will only result in small amounts of ridicule from the rest of the team.
- **L1 class:** This is a minor offense. There will not be any strict action taken on the maintainer such as kick/ban/mute. However some of the maintainers privileges as listed in Set of rules 7 can be taken away, except rule 1 in aforementioned Set of rules, for a specified period of time as per the discretion of the core team.
- **L2 class:** This is a major offense. The Maintainer will be held accountable which may lead to a temporary hold on all the privileges of the maintainers privileges as listed in Set of rules 7 can be taken away, except rule 1 in aforementioned Set of rules, for a specified period of time as per the discretion of the core team.
- **L3 class:** This is a critical offense. The Maintainer will either kicked/banned or muted in all rising related groups as per the discretion of the core team.

## Set of Rules: 0 - Community Rules

- **Rule 1:** Link shorteners that lead to advertisements are prohibited (L2)
- **Rule 2:** Maintainers can ask for donations for their hard work in their respective communities. Donation links are strictly prohibited in the posts on the Rising OS channel. (L1)
- **Rule 3:** Any developer can make and release builds in their respective device communities regardless of that device having official status. This is to prove our belief in open source where everyone can see and build for themselves. There can be no allegations or disputes between the official maintainer and community developers for limiting their freedom to build and post. (L3)

## Set of Rules: 1 - Common Sense Rules

- **Rule 1:** Maintainers must behave and treat all maintainers and core members respectfully when it is required for. Blatant remarks against of the team without any reasoning will lead to strict actions. (L2)
- **Rule 2:** Maintainers must treat all users with respect and listen to their problems & opinions. (L1 and if severe, L2)
- **Rule 3:** Maintainers must maintain a good reputation among fellow developers of their community if the community itself is good and respectful. (L2)

## Set of Rules: 2 - The Build Rules

- **Rule 1:** Maintainers cannot modify any part of the ROM source code while labeling it as an official release (Beta/community versions with source changes are permitted). (L2)
- **Rule 1.1:** Modifications to ROM sources are permitted only if explicitly allowed (following a discussion with the core team), primarily to support the device rather than to add features.
- **Rule 2:** The device tree must not contain changes that interfere with core features or CI build system. (L2)
- **Rule 3:** The kernel provided with the ROM must be open-source in compliance with GPLv3. (L3)
- **Rule 4:** Maintainers are prohibited from blocking any source side functionality in their builds. (L2)

## Set of Rules: 3 - The Release Rules

- **Rule 1:** Maintainers must upload their build and wait for it to be mirrored before making it available via OTA by making a pull request to the projects OTA repo or to releasing it as official. (L3)
- **Rule 1.1:** Only builds uploaded to the project's SourceForge or another host that is under the projects control can be shipped as official builds. Maintainers are strictly prohibited from using their own storage for official builds. (L3)
- **Rule 1.2:** The only exception to rule 1 and any subsections of it is an unofficial build of any kind.
- **Rule 2:** Maintainers reserve the right to re-release or take down builds at any time.
- **Rule 3:** Builds must be tested before release. (L3)
- **Rule 4:** Maintainers can release upto 2 builds for each device in a time period of 1 month. If any more is required, permission from the core team is required. This is to ensure quality rather than quantity.

## Set of Rules: 4 - The Trees Rules

- **Rule 1:** Device trees must be maintained in the device organization. If required, they can keep it private after notifing the core team with the reason. The exception to this being repos on any of the LineageOS organizations or AOSP git directly. (L3)
- **Rule 2:** Maintainers must test code before pushing it to the devive organization. Pushing wip changes can be done on a WIP branch. (L2)
- **Rule 3:** Maintainers must use "fifteen" as the branch name for A15 device trees. (L0)
- **Rule 4:** The device tree must not contain changes that interfere with core features or CI build system. (L2)
- **Rule 5:** The kernel provided with the ROM must be open-source in compliance with GPLv3. (L3)
- **Rule 6:** Maintainers must retain authorship of commits. Force-pushes are allowed. In addition, there can be no vendorsetup.sh files for cloning additional trees. (L2)
- **Rule 7:** Maintainers are prohibited from blocking any functionality using code that is or is similar to Boeffla Wakelock Blocker in their builds. (L3)
- **Rule 8:** Maintainers are prohibited from making SELinux permissive or disabling data encryption. In addition, sepolicy neverallows must never be ignored. (L3)
- **Rule 9:** There can be no unnecessary kernel modules such as kernel su included with the builds. (L2)
- **Rule 10:** Any device side code pushed to the projects git must not contain copyrighted blobs (e.g., megvii). If you for some reason require any such files, please conact the core team. <!--- Im looking right at you tecno mfs -->(L2)

## Set of Rules: 5 - The Languages Rules

- **Rule 1:** Maintainers must communicate in English in a clear and understandable manner.
- **Rule 2:** English shall be the primary language for communication with users.

## Set of Rules: 6 - The Group Rules

- **Rule 1:** Maintainers are prohibited from forwarding messages from the Maintainer Group without the sender's consent. (L1 or in extreme cases, L2)
- **Rule 2:** Core Members are prohibited from forwarding messages from the Core Group to Maintainer Group or elsewhere without the sender's consent. (L1 or in extreme cases, L2)

## Set of Rules: 7 - The Rights Rules

- **Rule 1:** Maintainers have the right to be treated with respect and dignity.
- **Rule 2:** Maintainers have the right to vote and express their opinions, in a respectful manner.
- **Rule 3:** Maintainers have the right to leave the project for any reason.
- **Rule 4:** Maintainers have the right to request for administrator privileges for the Rising OS general group.
- **Rule 5:** Maintainers have the right to contact any member of the core team, for any reason related to the project.
- **Rule 6:** Maintainers have the right to ask for any build to be taken down or reinstated in case of some unforceen issues cropping up.

## Set of Rules: 8 - The Group Rules

- **Rule 1:** Maintainers may create their own device groups using the format `RisingOS-{codename}` or use their device groups to provide support to the users of their devices.
- **Rule 2:** The group link used in the RisingOS channel posts so users can get support for the device must not contain any explicit material or content that is against the law. The same applies to any group operated by RisingOS team, included but not limited to RisingOS Support Group, Builders Group and Maintainers Group. (L2 and if severe, L3)
- **Rule 3 :** Device groups must be actively maintained and updated regularly to ensure community engagement and support. (L0 or L1)

## Extras

### These rules will take effect from the Android 16 release cycle. Please be aware of them as well so they dont surprise you later.

## Set of Rules: 3 - The Release Rules

- **Rule 1:** Maintainers must be aware that the RisingOS CI will automatically build and upload official builds automatically on a set schedule. This is to aim towards increasing the quality of our work via more strict source control. (L0)
- **Rule 1.1:** Maintainers must not ship official builds that they build on their local machine. Beta or unofficial or community builds are completely OK. (L2)
- **Rule 1.2:** Maintainers can be exempt from Rule 1.1 provided they have the permission from the core team. This permission requires a valid proper reasoning and is at the discretion of the entire core team.
