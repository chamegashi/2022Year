<script lang="ts">
  import * as genshinData from "../../public/genshin.json"
  import * as prosekaData from "../../public/proseka.json"
  import * as weaponData from "../../public/weapon.json"
  import * as youtubeData from "../../public/youtube.json"

  import type {CharaContent, WeaponContent, ProsekaContent, YoutubeContent} from "../../lib/types/contentDataType"

  const charactors: CharaContent[] = genshinData["default"];
  const prosekas: ProsekaContent[] = prosekaData["default"];
  const weapons: WeaponContent[] = weaponData["default"];
  const youtubes: YoutubeContent[] = youtubeData["default"];

  const showCharactor: CharaContent = charactors[Math.floor(Math.random() * charactors.length)]
  const showProseka: ProsekaContent = prosekas[Math.floor(Math.random() * prosekas.length)]
  const showWeapon: WeaponContent = weapons[Math.floor(Math.random() * weapons.length)]
  const showYoutube: YoutubeContent = youtubes[Math.floor(Math.random() * youtubes.length)]

</script>

<main class="bg-fixed h-screen" style="background-image: url(resultBack.jpg)">
  <div class="bg-fixed" style="background-image: url(fubuki.gif)">
    <div class="text-center text-3xl p-3 text-white font-semibold">あなたの今年のおすすめ！</div>
    <div class="flex-wrap flex justify-center">
  
      <div class="mb-4 mx-2 w-5/12 h-60">
        <div class="text-center m-2 text-xl text-white font-semibold ">原神オススメ</div>
        <div class="rounded border bg-white">
          <div class="flex justify-center">
            <img class="object-cover m-3 w-10/12 h-40 rounded" src={"genshin/" + showCharactor.file} alt={showCharactor.name} />
          </div>
          <div class="text-xl text-center font-semibold pb-1">{showCharactor.name}</div>
        </div>
      </div>
    
      <div class="mb-4 mx-2 w-5/12 h-60">
        <div class="text-center m-2 text-xl text-white font-semibold ">武器オススメ</div>
        <div class="rounded border bg-white">
          <div class="flex justify-center">
            <img class="object-contain m-3 w-10/12 h-40 rounded" src={"weapon/" + showWeapon.file} alt={showWeapon.name} />
          </div>
          <div class="text-xl text-center font-semibold pb-1">{showWeapon.name}</div>
        </div>
      </div>
  
      <div class="my-2 mx-3 w-11/12">
        <div class="text-center m-2 text-xl text-white font-semibold ">プロセカオススメ</div>
        <div class="rounded border bg-white">
          <div class="flex justify-center">
            <img class="object-contain w-10/12 h-44 rounded" src={"proseka/" + showProseka.file} alt={showProseka.name} />
          </div>
        </div>
      </div>
  
      <div class="mx-3 w-10/12 h-60">
        <div class="text-center m-2 text-xl text-white font-semibold ">ボカロオススメ</div>
        <div class="rounded border bg-white">
          <div class="flex justify-center m-2">
            <iframe 
              width="400"
              height="170"
              src={showYoutube.url}
              title="YouTube video player"
              frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
              allowfullscreen
            >
            </iframe>
          </div>
          <div class="text-xl text-center font-semibold pb-1">{showYoutube.title}</div>
        </div>
      </div>
  
    </div>
  </div>
</main>