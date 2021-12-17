<script lang="ts">
  export let name: string;
</script>

<main class="bg-fixed h-screen" style="background-image: url(resultBack.jpg)">
  <div class="bg-fixed h-screen" style="background-image: url(fubuki.gif)">
    <div class="text-center text-4xl p-3 text-white font-semibold">あなたの今年のおすすめ！</div>
    <div class="flex-wrap flex justify-center">
  
      <div class="my-4 mx-3 w-5/12 h-60">
        <div class="text-center m-2 text-xl text-white font-semibold ">原神オススメ</div>
        <div class="rounded border bg-white">
          <div class="flex justify-center">
            <img class="object-cover m-3 w-10/12 h-40" src="genshin/ジン.png" alt="ジン" />
          </div>
          <div class="text-xl text-center font-semibold pb-1">ジン</div>
        </div>
      </div>
    
      <div class="my-4 mx-3 w-5/12 h-60">
        <div class="text-center m-2 text-xl text-white font-semibold ">武器オススメ</div>
        <div class="rounded border bg-white">
          <div class="flex justify-center">
            <img class="object-contain m-3 w-10/12 h-40" src="weapon/ランページ.png" alt="ランページ" />
          </div>
          <div class="text-xl text-center font-semibold pb-1">ランページ</div>
        </div>
      </div>
  
      <div class="my-4 mx-3 w-11/12 h-60">
        <div class="text-center m-2 text-xl text-white font-semibold ">プロセカオススメ</div>
        <div class="rounded border bg-white">
          <div class="flex justify-center">
            <img class="object-contain m-3 w-10/12 h-48" src="proseka/宵崎奏.jpg" alt="宵崎奏.jpg" />
          </div>
        </div>
      </div>
  
      <div class="my-4 mx-3 w-10/12 h-60">
        <div class="text-center m-2 text-xl text-white font-semibold ">ボカロオススメ</div>
        <div class="rounded border bg-white">
          <div class="flex justify-center m-2">
            <iframe 
              width="400"
              height="200"
              src="https://www.youtube.com/embed/y3YuIvHYBt8"
              title="YouTube video player"
              frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
              allowfullscreen
            >
            </iframe>
          </div>
          <div class="text-xl text-center font-semibold pb-1">偽物人間40号</div>
        </div>
      </div>
  
    </div>
  </div>
</main>