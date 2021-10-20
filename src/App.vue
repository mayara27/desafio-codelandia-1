<template>
  <div id="app">
    <nav class="nav">
      <p class="title template-title">Codelândia</p>
      <p class="blog template-title">blog</p>
        <v-icon class="icon-ajusts"
          large
          color="rgba(255, 255, 255)">
          mdi-magnify
        </v-icon>
      <input type="text" class="search" placeholder="Pesquisar no blog">
    </nav>

    <div class="conteudo">
      <Publication :pubs="pubs" />
    </div>
  </div>
</template>

<script>
import Publication from './components/Publication.vue'
export default {
  components: { Publication }, 
  name: 'App',
  data() {
		return {
			pubs: [
				{date: '19 de out, 21', title: 'Agora é oficial: o Windows 11 está vindo', body: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor eleifend lectus non, vestibulum nulla. Aliquam euismod enim sit amet tortor viverra sagittis. Donec nulla nulla, hendrerit quis eros eget, bibendum maximus ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, "
        },
        {date: '20 de out, 21', title: 'Tim Berners-Lee vai leiloar código-fonte da web', body: "lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, "
        },
        {date: '20 de out, 21', title: 'Tem Firefox novo no pedaço e você vai querer migrar', body: "lorem, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, "
        },
        {date: '20 de out, 21', title: 'John McAfee, criador do antivírus McAfee, morre', body: "Lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, lorem hsua çelmf dnsklc nsidma ex.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla quis libero porttitor, "
        },        
			]
		}
	},
}
</script>

<style >

  body {
		font-family: 'Lato', sans-serif;
		background: rgb(235, 235, 235);
		color: #FFF;
	}

	.nav {
    position: absolute;
    width: 100%;
    height: 250px;
    left: 0px;
    top: 0px;
    background: linear-gradient(90deg, #574AE8 0%, #3EA1DB 100%);		
	}

  .template-title {
    font-family: Lexend Deca;
    font-style: normal;
    font-weight:400;
    font-size: 24px;
    line-height: 30px;
    color: #FFFFFF;
    text-align: right;
  }
  .title {
    position: absolute;
    width: 133px;
    height: 30px;
    left: 13%;
    top: 41px;
  }

  .blog {
    position: absolute;
    width: 52px;
    height: 30px;
    right: 15%;
    top: 41px;
  }

  .search {
    position: absolute;
    width: 75%;
    height: 65px;
    left: 13%;
    right: 15%;
    top: 144px;
    border: none;
    background: rgba(255, 255, 255, 0.4);
    border-radius: 5px;
    outline: 0;
  }

  input.search {
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    line-height: 22px;
    text-align: left;
    color: #FFFFFF;
    opacity: 0.5;
    padding-left: 60px;
  }

  input::placeholder {
    color: #FFFFFF; 
  }

  .icon-ajusts {
    height: 65px;
    left: 14%;
    right: 15%;
    top: 144px;
  }

  .conteudo{
    position: relative;
    top: 350px;
  }

</style>
