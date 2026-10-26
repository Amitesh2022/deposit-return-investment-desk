<script setup lang="ts">
import { onMounted } from 'vue'
import { storeToRefs } from 'pinia'
import { RouterLink, RouterView } from 'vue-router'
import { useDeliveryStore } from './store'
const store = useDeliveryStore()
const { approvedShare, offers, urgent } = storeToRefs(store)
onMounted(store.load)
</script>

<template><div class="shell"><aside><div class="brand">ReturnLoopEU<span>CIRCULAR PACKAGING</span></div><nav><RouterLink to="/">Return schemes</RouterLink><RouterLink to="/insights">System guidance</RouterLink></nav><div class="health"><i /> Java deposit return investment service connected</div></aside><main><header><div><span class="eyebrow">Scale high-performing packaging return systems</span><h1>Deposit Return Investment Desk</h1></div><button @click="store.addOffer">Add return scheme</button></header><section class="summary"><article><small>Schemes ready</small><strong>{{ approvedShare }}%</strong><div class="bar"><span :style="{ width: `${approvedShare}%` }" /></div></article><article><small>Schemes tracked</small><strong>{{ offers.length }}</strong><p>Shared system view</p></article><article><small>High-priority gaps</small><strong>{{ urgent }}</strong><p>Needs attention</p></article></section><RouterView /></main></div></template>
