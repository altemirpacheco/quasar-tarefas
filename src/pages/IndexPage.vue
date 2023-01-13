<template>
  <q-page class="row">
    <q-card class="col-xs-6">
      <q-toolbar>
        <q-input
          borderless
          placeholder="Pesquisar"
          class="full-width"
          :model-value="buscar"
        ></q-input>
      </q-toolbar>
      <q-list>
        <q-item>
          <q-item-section side>
            <q-checkbox :model-value="true" />
          </q-item-section>
          <q-item-section>Tarefa 1</q-item-section>
          <q-item-section side>
            <q-btn flat icon="mdi-delete" round size="sm"></q-btn>
          </q-item-section>
        </q-item>
      </q-list>
    </q-card>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
  data() {
    return {
      buscar: "",
    };
  },
});
</script>
