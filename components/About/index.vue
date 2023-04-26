<script lang="ts">
import Vue, { PropOptions } from 'vue'

interface AboutData {
  title: string
  body: string
  actionUrl: string
  actionTitle: string
  image: string
}

export default Vue.extend({
  name: 'AboutComponent',
  props: {
    data: {
      type: Object,
      // required: true,
    } as PropOptions<AboutData>,
  },
})
</script>

<template>
  <div>
    <div class="container mx-auto px-6 flex items-center justify-between flex-col lg:flex-row">
      <div class="flex flex-col gap-8">
        <img
          class="w-20 xl:w-44"
          width="auto"
          height="auto"
          :src="require('~/assets/images/brand-symbol.png')"
          alt="Brand Symbol"
        />
        <h2 class="title max-w-[360px]">Para quem é a impulse</h2>
        <p class="text-cover max-w-[455px]">
          As melhores soluções pensadas para o seu negócio
        </p>
      </div>
      <ul class="flex flex-wrap flex-row justify-center gap-24 text-white p-6 max-w-[917px]">
        <li class="w-full lg:w-auto">
          <svg
            width="64"
            height="64"
            viewBox="0 0 64 64"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <mask
              id="mask0_127_46"
              style="mask-type: alpha"
              maskUnits="userSpaceOnUse"
              x="0"
              y="0"
              width="64"
              height="64"
            >
              <rect width="64" height="64" fill="#D9D9D9" />
            </mask>
            <g mask="url(#mask0_127_46)">
              <path
                d="M31.9999 30.2667C33.0221 30.2667 33.8781 29.9218 34.5679 29.232C35.2559 28.544 35.5999 27.6889 35.5999 26.6666C35.5999 25.6444 35.2559 24.7884 34.5679 24.0986C33.8781 23.4106 33.0221 23.0666 31.9999 23.0666C30.9777 23.0666 30.1226 23.4106 29.4346 24.0986C28.7448 24.7884 28.3999 25.6444 28.3999 26.6666C28.3999 27.6889 28.7448 28.544 29.4346 29.232C30.1226 29.9218 30.9777 30.2667 31.9999 30.2667ZM31.9999 54.7333C37.5999 49.9333 41.9555 44.9884 45.0666 39.8986C48.1777 34.8106 49.7332 30.5778 49.7332 27.2C49.7332 21.8222 48.0221 17.4329 44.5999 14.032C41.1777 10.6329 36.9777 8.93332 31.9999 8.93332C27.0221 8.93332 22.8221 10.6329 19.3999 14.032C15.9777 17.4329 14.2666 21.8222 14.2666 27.2C14.2666 30.5778 15.8221 34.8106 18.9332 39.8986C22.0443 44.9884 26.3999 49.9333 31.9999 54.7333ZM31.9999 57.3333C25.3777 51.3778 20.4559 45.8551 17.2346 40.7653C14.0115 35.6773 12.3999 31.1555 12.3999 27.2C12.3999 21.0666 14.3777 16.1778 18.3332 12.5333C22.2888 8.88887 26.8443 7.06665 31.9999 7.06665C37.1555 7.06665 41.711 8.88887 45.6666 12.5333C49.6221 16.1778 51.5999 21.0666 51.5999 27.2C51.5999 31.1555 49.9892 35.6773 46.7679 40.7653C43.5448 45.8551 38.6221 51.3778 31.9999 57.3333Z"
                fill="white"
              />
            </g>
          </svg>

          <h3
            class="font-title text-3xl uppercase text-light h-[78px] my-6 flex items-end"
          >
            <span>
              Negócios<br />
              locais e <span class="text-[#F2632D]">MEI</span>
            </span>
          </h3>
          <p
            class="font-light text-white/50 mt-8 leading-[26px] lg:w-[220px] lg:max-w-[220px]"
          >
            Para você que precisa gerar mais tráfego para o seu negócio local,
            captar mais leads qualificados e fortalecer o posicionamento da sua
            marca, considerando os hábitos de consumo da audiência na sua
            cidade.
          </p>
        </li>
        <li>
          <svg
            width="64"
            height="64"
            viewBox="0 0 64 64"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <mask
              id="mask0_127_52"
              style="mask-type: alpha"
              maskUnits="userSpaceOnUse"
              x="0"
              y="0"
              width="64"
              height="64"
            >
              <rect width="64" height="64" fill="#D9D9D9" />
            </mask>
            <g mask="url(#mask0_127_52)">
              <path
                d="M13.7334 52.5333C12.5778 52.5333 11.6223 52.1556 10.8667 51.4C10.1112 50.6444 9.7334 49.6889 9.7334 48.5333V15.4667C9.7334 14.3111 10.1112 13.3556 10.8667 12.6C11.6223 11.8444 12.5778 11.4667 13.7334 11.4667H38.8001V13.3333H13.7334C13.1112 13.3333 12.6001 13.5333 12.2001 13.9333C11.8001 14.3333 11.6001 14.8444 11.6001 15.4667V48.5333C11.6001 49.1556 11.8001 49.6667 12.2001 50.0667C12.6001 50.4667 13.1112 50.6667 13.7334 50.6667H46.8001C47.4223 50.6667 47.9334 50.4667 48.3334 50.0667C48.7334 49.6667 48.9334 49.1556 48.9334 48.5333V23.4667H50.8001V48.5333C50.8001 49.6889 50.4223 50.6444 49.6667 51.4C48.9112 52.1556 47.9556 52.5333 46.8001 52.5333H13.7334ZM19.4667 43.6H21.3334V28.4H19.4667V43.6ZM29.3334 43.6H31.2001V20.4H29.3334V43.6ZM39.2001 43.6H41.0667V36.4H39.2001V43.6ZM47.0667 20.5333V15.2H41.7334V13.3333H47.0667V8H48.9334V13.3333H54.2667V15.2H48.9334V20.5333H47.0667Z"
                fill="white"
              />
            </g>
          </svg>

          <h3
            class="font-title text-3xl uppercase w-[237px] h-[78px] my-6 flex items-end"
          >
            <span>
              Marcas que<br />
              buscam <span class="text-[#F2632D]">+ resultados</span>
            </span>
          </h3>
          <p
            class="font-light text-white/50 leading-[26px] lg:w-[220px] lg:max-w-[220px]"
          >
            Para marcas que buscam uma estratégia em busca de resultados através
            de soluções inovadoras. Conquiste definitivamente sua autoridade no
            mercado digital e conquiste mais clientes.
          </p>
        </li>
        <li>
          <svg
            width="64"
            height="64"
            viewBox="0 0 64 64"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <mask
              id="mask0_127_58"
              style="mask-type: alpha"
              maskUnits="userSpaceOnUse"
              x="0"
              y="0"
              width="64"
              height="64"
            >
              <rect width="64" height="64" fill="#D9D9D9" />
            </mask>
            <g mask="url(#mask0_127_58)">
              <path
                d="M19.7333 55.6C18.7111 55.6 17.856 55.2551 17.168 54.5653C16.4782 53.8773 16.1333 53.0222 16.1333 52C16.1333 50.9778 16.4782 50.1227 17.168 49.4347C17.856 48.7449 18.7111 48.4 19.7333 48.4C20.7555 48.4 21.6115 48.7449 22.3013 49.4347C22.9893 50.1227 23.3333 50.9778 23.3333 52C23.3333 53.0222 22.9893 53.8773 22.3013 54.5653C21.6115 55.2551 20.7555 55.6 19.7333 55.6ZM44.2666 55.6C43.2444 55.6 42.3893 55.2551 41.7013 54.5653C41.0115 53.8773 40.6666 53.0222 40.6666 52C40.6666 50.9778 41.0115 50.1227 41.7013 49.4347C42.3893 48.7449 43.2444 48.4 44.2666 48.4C45.2889 48.4 46.144 48.7449 46.832 49.4347C47.5217 50.1227 47.8666 50.9778 47.8666 52C47.8666 53.0222 47.5217 53.8773 46.832 54.5653C46.144 55.2551 45.2889 55.6 44.2666 55.6ZM15.4666 14.2667L22.8 29.7333H40.2C40.6 29.7333 40.9555 29.6329 41.2666 29.432C41.5777 29.2329 41.8444 28.9555 42.0666 28.6L48.9333 16.1333C49.2 15.6444 49.2222 15.2106 49 14.832C48.7777 14.4551 48.4 14.2667 47.8666 14.2667H15.4666ZM14.5333 12.4H47.8666C49.0666 12.4 49.9662 12.8773 50.5653 13.832C51.1662 14.7884 51.2 15.7778 50.6666 16.8L43.6 29.7333C43.2444 30.3111 42.7893 30.7662 42.2346 31.0986C41.6782 31.4329 41.0666 31.6 40.4 31.6H21.6L18.2666 37.7333C17.9111 38.2667 17.9004 38.8444 18.2346 39.4667C18.5671 40.0889 19.0666 40.4 19.7333 40.4H47.8666V42.2667H19.7333C18.3111 42.2667 17.256 41.6782 16.568 40.5013C15.8782 39.3227 15.8666 38.1333 16.5333 36.9333L20.6666 29.6L10.8 8.93332H6.1333V7.06665H12L14.5333 12.4Z"
                fill="white"
              />
            </g>
          </svg>

          <h3
            class="font-title text-3xl uppercase h-[78px] my-6 flex items-end"
          >
            <span class="text-[#F2632D]"> Ecommerces </span>
          </h3>
          <p
            class="font-light text-white/50 leading-[26px] lg:w-[220px] lg:max-w-[220px]"
          >
            Para você que precisa desenvolver uma loja virtual, gerar mais
            tráfego e ampliar suas vendas no ambiente virtual.
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>
