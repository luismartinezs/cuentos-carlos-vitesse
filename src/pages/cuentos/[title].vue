<script>
import { useRouter } from 'vue-router'
import PapaNoel from '../../posts/papa-noel.md'

export default {
  components: {
    PapaNoel,
  },
  setup() {
    const router = useRouter()
    return { router }
  },
}
// import { useUserStore } from '~/stores/user'

// const props = defineProps<{ title: string }>()
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
      <button class="btn m-3 text-sm mt-6" @click="router.back()">
        Volver
      </button>
    </div>
  </div>
</template>
