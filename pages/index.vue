<template>
<!-- component -->
<section>
<base-header/>
<base-hero/>
<base-timeline/>
<base-testimonials/>
<base-pricing/>
<base-contact/>
</section>

</template>

<script>
import BasePricing from '~/components/BasePricing.vue'
import BaseTestimonials from '~/components/BaseTestimonials.vue'
import BaseContact from '~/components/BaseContact.vue'
import BaseHeader from '~/components/BaseHeader.vue'
import BaseTimeline from '~/components/BaseTimeline.vue'

export default {components: {
    BasePricing,
    BaseTestimonials,
    BaseContact,
    BaseHeader,
    BaseTimeline,

  },
  }
</script>

<style>

</style>
