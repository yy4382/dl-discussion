---
layout: page
---
<script setup>
import {
  VPTeamPage,
  VPTeamPageTitle,
  VPTeamMembers
} from 'vitepress/theme'

const members = [
  {
    avatar: 'https://avatars.githubusercontent.com/u/112888202',
    name: 'kiyotakali',
    links: [
      { icon: 'github', link: 'https://github.com/kiyotakali' },
    ]
  },
  {
    avatar: "https://avatars.githubusercontent.com/u/55980292",
    name: "yy4382",
    links: [
      { icon: 'github', link: 'https://github.com/yy4382' },
    ]
  }
]
</script>

<VPTeamPage>
  <VPTeamPageTitle>
    <template #title>
      Members
    </template>
    <template #lead>
      Members of our group.
    </template>
  </VPTeamPageTitle>
  <VPTeamMembers
    :members="members"
  />
</VPTeamPage>