<template>
  <main class="container py-5">
    <h1>{{ t('footerSwitchHelp.title') }}</h1>

    <p>
      {{ t('footerSwitchHelp.form.paragraph1') }}      
      <code>
        &lt;GenericFooter /&gt;
      </code>
      {{ t('footerSwitchHelp.form.paragraph2') }}
      <code>
        &lt;FooterBar /&gt;
      </code>.
    </p>

    <h4 class="mt-4">📁 {{ t('footerSwitchHelp.form.subtitle') }}
      <code>
        App.vue
      </code>
    </h4>

    <p>
      {{ t('footerSwitchHelp.form.paragraph3') }}
      <strong>
        <code>
          src/views/App.vue
        </code>
      </strong>
      {{ t('footerSwitchHelp.form.paragraph4') }}
    </p>

    <h4 class="mt-4">🔗{{ t('footerSwitchHelp.form.subtitle1') }}</h4>
    <p>{{ t('footerSwitchHelp.form.paragraph5') }}</p>

    <pre>
      <code>
        import FooterBar from "@/components/FooterBar.vue";
        import GenericFooter from "@/components/GenericFooter.vue";
      </code>
    </pre>

    <h4 class="mt-4">🧩{{ t('footerSwitchHelp.form.subtitle2') }}
      <code>
        &lt;template&gt;
      </code>
    </h4>

    <p>{{ t('footerSwitchHelp.form.paragraph6') }} `App.vue`:</p>

    <pre>
      <code>
        &lt;!-- {{ t('footerSwitchHelp.form.paragraph7') }} --&gt;
        &lt;!-- &lt;GenericFooter /&gt; --&gt;
        &lt;FooterBar /&gt;
      </code>
    </pre>

    <p>{{ t('footerSwitchHelp.form.paragraph8') }}</p>

    <ul>
      <li>
        <strong>
          {{ t('footerSwitchHelp.form.paragraph9') }}
          <code>
            GenericFooter
          </code>
          :
        </strong>
      </li>
    </ul>

    <pre>
      <code>
        &lt;GenericFooter /&gt;
        &lt;!-- &lt;FooterBar /&gt; --&gt;
      </code>
    </pre>

    <ul>
      <li>
        <strong>
          {{ t('footerSwitchHelp.form.paragraph9') }}
          <code>
            FooterBar
          </code>
          :
        </strong>
      </li>
    </ul>

    <pre>
      <code>
        &lt;!-- &lt;GenericFooter /&gt; --&gt;
        &lt;FooterBar /&gt;
      </code>
    </pre>

    <h4 class="mt-4">✅ {{ t('footerSwitchHelp.form.subtitle3') }}
      <code>
        &lt;GenericFooter /&gt;
      </code>
    </h4>

    <pre>
      <code>
        &lt;template&gt;
          &lt;div id="app" class="d-flex flex-column min-vh-100"&gt;
            &lt;Navbar /&gt;
            &lt;main class="flex-fill container py-4"&gt;
              &lt;RouterView /&gt;
            &lt;/main&gt;
            &lt;GenericFooter /&gt;
            &lt;!-- &lt;FooterBar /&gt; --&gt;
          &lt;/div&gt;
        &lt;/template&gt;

        &lt;script setup lang="ts"&gt;
          import Navbar from "@/components/NavBar.vue";
          import FooterBar from "@/components/FooterBar.vue";
          import GenericFooter from "@/components/GenericFooter.vue";
        &lt;/script&gt;
      </code>
    </pre>

    <p class="mt-4 text-muted">
      {{ t('footerSwitchHelp.form.paragraph10') }}
    </p>
  </main>
</template>

<script setup lang="ts">
import { useI18n } from 'vue-i18n';
const { t } = useI18n();
</script>
