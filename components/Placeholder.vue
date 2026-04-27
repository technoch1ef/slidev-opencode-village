<script setup lang="ts">
/**
 * Placeholder.vue
 *
 * Renders a styled placeholder box for screenshot / diagram slots.
 * Usage in slides: <Placeholder label="Architecture Diagram" />
 */
withDefaults(
  defineProps<{
    /** Text shown inside the box */
    label?: string
    /** Box height (CSS value) */
    height?: string
    /** Box width (CSS value) */
    width?: string
  }>(),
  {
    label: 'Placeholder',
    height: '200px',
    width: '100%',
  },
)
</script>

<template>
  <div class="placeholder-box" :style="{ height, width }">
    <span class="placeholder-label">{{ label }}</span>
  </div>
</template>

<style scoped>
.placeholder-box {
  display: flex;
  align-items: center;
  justify-content: center;
  border: 2px dashed var(--vivid-muted, #595C66);
  border-radius: 8px;
  background: rgba(87, 182, 255, 0.04);
  margin: 1em 0;
}

.placeholder-label {
  color: var(--vivid-comment, #696C76);
  font-size: 0.95em;
  font-style: italic;
  text-transform: uppercase;
  letter-spacing: 0.08em;
}
</style>
