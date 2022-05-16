---
lang: en-US
title: Details
---

# Project Details View

This is a detailed view of the project. Here you find all relevant information.

| Name      | Value                                       |
|-----------|---------------------------------------------|
| Full Name | {{ siteData.variables?.project?.fullName }} |
| Job Title | {{ siteData.variables?.project?.job }}      |
| Email     | {{ siteData.variables?.project?.email }}    |
| Salary    | {{ siteData.variables?.project?.salary }}   |
| About     | {{ siteData.variables?.project?.about }}    |


<script setup lang="ts">
import { useSiteData } from '@vuepress/client'

const siteData = useSiteData()
</script>