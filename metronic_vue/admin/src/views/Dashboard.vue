<template>
  <!--begin::Row-->
  <div class="row g-5 g-xl-8">
    <!--begin::Col-->
    <div class="col-xl-4">
      <MixedWidget1
        widget-classes="card-xl-stretch mb-xl-8"
        widget-color="primary"
      ></MixedWidget1>
    </div>
    <!--end::Col-->

    <!--begin::Col-->
    <div class="col-xl-4">
      <MixedWidget1
        widget-classes="card-xl-stretch mb-xl-8"
        widget-color="danger"
      ></MixedWidget1>
    </div>
    <!--end::Col-->

    <!--begin::Col-->
    <div class="col-xl-4">
      <MixedWidget1
        widget-classes="card-xl-stretch mb-5 mb-xl-8"
        widget-color="success"
      ></MixedWidget1>
    </div>
    <!--end::Col-->
  </div>
  <!--end::Row-->

  <!--begin::Row-->
  <div class="row g-5 g-xl-8">
    <!--begin::Col-->
    <div class="col-xl-4">
      <MixedWidget2
        widget-classes="card-xl-stretch mb-xl-8"
        widget-color="info"
        chart-height="200"
        stroke-color="#4e12c4"
      ></MixedWidget2>
    </div>
    <!--end::Col-->

    <!--begin::Col-->
    <div class="col-xl-4">
      <MixedWidget2
        widget-classes="card-xl-stretch mb-xl-8"
        widget-color="danger"
        chart-height="200"
        stroke-color="#cb1e46"
      ></MixedWidget2>
    </div>
    <!--end::Col-->

    <!--begin::Col-->
    <div class="col-xl-4">
      <MixedWidget2
        widget-classes="card-xl-stretch mb-xl-8"
        widget-color="primary"
        chart-height="200"
        stroke-color="#0078d0"
      ></MixedWidget2>
    </div>
    <!--end::Col-->


  
  </div>
  <!--end::Row-->
</template>

<script lang="ts">
import { getAssetPath } from "@/core/helpers/assets";
import { defineComponent } from "vue";
import MixedWidget1 from "@/components/widgets/mixed/Widget1.vue";
import MixedWidget2 from "@/components/widgets/mixed/Widget2.vue";
import MixedWidget3 from "@/components/widgets/mixed/Widget3.vue";
import MixedWidget4 from "@/components/widgets/mixed/Widget4.vue";
import MixedWidget5 from "@/components/widgets/mixed/Widget5.vue";
import MixedWidget6 from "@/components/widgets/mixed/Widget6.vue";


export default defineComponent({
  name: "Dashboard",
  components: {
    MixedWidget1,
    MixedWidget2,
    MixedWidget3,
    MixedWidget4,
    MixedWidget5,
    MixedWidget6
  },
  setup() {
    return {
      getAssetPath,
    };
  },
});
</script>
