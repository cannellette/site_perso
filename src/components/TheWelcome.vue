<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
 
 <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Mon CV</template>

    Téléchargez mon 
    <a href="/CannelleGarcia.png" download>CV</a>.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Mon Github</template>

  
    Pour retrouver mes projets collectifs, individuels et mes katas : <a href="https://github.com/cannellette" target="_blank" rel="noopener">C'est par ici que ça se passe</a>!

    <br />

  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Linkedin</template>

    Retrouvez-moi sur<a href="https://www.linkedin.com/in/cannelle-garcia/" target="_blank" rel="noopener">Linkedin </a>! 

  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Mes projets</template>

    Retrouvez ici mes<a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">projets</a>.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Contact</template>

    Contactez-moi <a href="mailto:cannelle.garcia@gmail.com" target="_blank" rel="noopener">par mail</a> !
  </WelcomeItem>




</template>
<script>
export default {
  methods: {
    openAndDownloadImage(event) {
      event.preventDefault();
      const imageUrl = './assets/CannelleGarcia.png';
      window.open(imageUrl, '_blank');
      location.href = imageUrl;
    },
  },
};
</script>