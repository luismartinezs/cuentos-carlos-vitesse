<script setup lang="ts">
import PapaNoel from '../../posts/papa-noel.md'
// import { useUserStore } from '~/stores/user'

// const props = defineProps<{ name: string }>()
// const router = useRouter()
// const user = useUserStore()
// const { t } = useI18n()

// watchEffect(() => {
//   user.setNewName(props.title)
// })
</script>

<template>
  <div>
    <PapaNoel />
    <div>
      <button
        class="btn m-3 text-sm mt-6"
        @click="router.back()"
      >
        {{ t('button.back') }}
      </button>
    </div>
  </div>
</template>
