<script setup lang="ts">
import { h } from "vue";
import { NDataTable, NButton } from 'naive-ui';
import type { DataTableColumns } from 'naive-ui';
import router from "../router";

type ConversationItem = {
    name: string,
    title: string,
    messages: number
}

const data = [
  { name: "Furious, In-Alt", title: "Free Will and Moral Luck", messages: 4 },
  { name: "In-Alt, Furious", title: "The Evolution of Tumblr Discourse", messages: 14 },
  { name: "Furious, In-Alt", title: "The Objectivity of Fun, as Experienced by Kitties", messages: 9 },
  { name: "In-Alt, Furious", title: "Religion as a Moral Fiction", messages: 7 }
];

const columns: DataTableColumns<ConversationItem> = [
      {
        title: 'Name',
        key: 'name'
      },
      {
        title: 'Title',
        key: 'title'
      },
      {
        title: 'Messages',
        key: 'messages'
      },
      {
        title: "",
        key: 'actions',
        render (row) {
            return h(
            NButton,
            {
                size: 'tiny',
                onClick: () => router.push('/')
            },
            { default: () => 'View' }
            )
        }
      }
    ]
</script>

<template>
  <NDataTable
    :columns="columns"
    :data="data"
    :pagination="false"
  />
</template>