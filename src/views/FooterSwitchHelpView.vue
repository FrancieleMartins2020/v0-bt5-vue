<template>
  <main class="container py-5">
    <h1>Como alternar entre rodapés no Vue</h1>

    <p>
      Este projeto possui dois componentes de rodapé que podem ser usados conforme sua preferência:
      <code>&lt;GenericFooter /&gt;</code> e <code>&lt;FooterBar /&gt;</code>.
    </p>

    <h4 class="mt-4">📁 Passo 1: Localize o arquivo <code>App.vue</code></h4>
    <p>
      Vá até a pasta <strong><code>src/views/App.vue</code></strong>. Este é o componente raiz da sua aplicação.
    </p>

    <h4 class="mt-4">🔗 Passo 2: Verifique os imports</h4>
    <p>No início do arquivo, devem estar importados os dois rodapés:</p>

    <pre><code>import FooterBar from "@/components/FooterBar.vue";
import GenericFooter from "@/components/GenericFooter.vue";</code></pre>

    <h4 class="mt-4">🧩 Passo 3: Altere o rodapé desejado no <code>&lt;template&gt;</code></h4>

    <p>Você encontrará algo assim no final do `App.vue`:</p>

    <pre><code>&lt;!-- Criar rodapé --&gt;
&lt;!-- &lt;GenericFooter /&gt; --&gt;
&lt;FooterBar /&gt;</code></pre>

    <p>Para alternar entre os componentes, comente um e descomente o outro:</p>

    <ul>
      <li><strong>Para usar o <code>GenericFooter</code>:</strong></li>
    </ul>
    <pre><code>&lt;GenericFooter /&gt;
&lt;!-- &lt;FooterBar /&gt; --&gt;</code></pre>

    <ul>
      <li><strong>Para usar o <code>FooterBar</code>:</strong></li>
    </ul>
    <pre><code>&lt;!-- &lt;GenericFooter /&gt; --&gt;
&lt;FooterBar /&gt;</code></pre>

    <h4 class="mt-4">✅ Exemplo completo com <code>&lt;GenericFooter /&gt;</code></h4>

        <pre><code>&lt;template&gt;
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
    &lt;/script&gt;</code></pre>

    <p class="mt-4 text-muted">
      Com isso, você consegue alternar visualmente qual rodapé deseja exibir em sua aplicação Vue.
    </p>
  </main>
</template>

<script setup lang="ts">
</script>
