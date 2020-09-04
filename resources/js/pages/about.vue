<template>
  <div>
    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Architecto soluta
    vero dignissimos nobis modi autem alias laborum nesciunt, ex facilis! Error
    obcaecati, laudantium impedit officiis ratione facilis accusamus tenetur
    unde aut soluta dolore voluptatibus, perspiciatis officia rem repellendus
    possimus, accusantium nesciunt. Recusandae libero temporibus, beatae
    sapiente doloremque aut magnam reprehenderit numquam explicabo, harum odio
    sed ad nihil vel id cupiditate neque ipsa omnis. Vel corrupti laboriosam
    consectetur labore fugiat earum deleniti similique quibusdam soluta
    consequatur aliquam omnis, dicta fugit nemo aspernatur laudantium hic,
    voluptatibus quas maxime ratione eaque! Quibusdam veritatis ipsam aliquam
    distinctio sequi eveniet nostrum iusto quam illo praesentium voluptates
    ullam facilis ipsa, consectetur modi tenetur aut libero voluptatibus! A,
    culpa amet mollitia iste minus consequatur laborum eligendi est veritatis
    officiis adipisci provident excepturi deserunt illum quo velit id sunt
    veniam pariatur nostrum maiores porro tempore molestiae. Quo ea, optio,
    possimus minima placeat perferendis soluta accusamus, quasi qui itaque error
    provident fugiat sunt architecto inventore doloribus esse explicabo
    excepturi laborum quam numquam atque quaerat velit? Iusto aspernatur dolores
    minus inventore doloribus repellendus obcaecati vitae earum delectus tenetur
    deserunt officia officiis animi dolorum omnis doloremque quibusdam sint,
    harum similique cum cumque iure sapiente ullam beatae. Ipsa magnam a beatae
    dignissimos.

    <div>
      <button v-tooltip="{ content: 'You have ' + 3 + ' new messages.' }">
        Count
      </button>
    </div>
  </div>
</template>

<script></script>

<style>
.tooltip {
  display: block !important;
  z-index: 10000;
}

.tooltip .tooltip-inner {
  background: black;
  color: white;
  border-radius: 16px;
  padding: 5px 10px 4px;
}

.tooltip .tooltip-arrow {
  width: 0;
  height: 0;
  border-style: solid;
  position: absolute;
  margin: 5px;
  border-color: black;
  z-index: 1;
}

.tooltip[x-placement^="top"] {
  margin-bottom: 5px;
}

.tooltip[x-placement^="top"] .tooltip-arrow {
  border-width: 5px 5px 0 5px;
  border-left-color: transparent !important;
  border-right-color: transparent !important;
  border-bottom-color: transparent !important;
  bottom: -5px;
  left: calc(50% - 5px);
  margin-top: 0;
  margin-bottom: 0;
}

.tooltip[x-placement^="bottom"] {
  margin-top: 5px;
}

.tooltip[x-placement^="bottom"] .tooltip-arrow {
  border-width: 0 5px 5px 5px;
  border-left-color: transparent !important;
  border-right-color: transparent !important;
  border-top-color: transparent !important;
  top: -5px;
  left: calc(50% - 5px);
  margin-top: 0;
  margin-bottom: 0;
}

.tooltip[x-placement^="right"] {
  margin-left: 5px;
}

.tooltip[x-placement^="right"] .tooltip-arrow {
  border-width: 5px 5px 5px 0;
  border-left-color: transparent !important;
  border-top-color: transparent !important;
  border-bottom-color: transparent !important;
  left: -5px;
  top: calc(50% - 5px);
  margin-left: 0;
  margin-right: 0;
}

.tooltip[x-placement^="left"] {
  margin-right: 5px;
}

.tooltip[x-placement^="left"] .tooltip-arrow {
  border-width: 5px 0 5px 5px;
  border-top-color: transparent !important;
  border-right-color: transparent !important;
  border-bottom-color: transparent !important;
  right: -5px;
  top: calc(50% - 5px);
  margin-left: 0;
  margin-right: 0;
}

.tooltip.popover .popover-inner {
  background: #f9f9f9;
  color: black;
  padding: 24px;
  border-radius: 5px;
  box-shadow: 0 5px 30px rgba(black, 0.1);
}

.tooltip.popover .popover-arrow {
  border-color: #f9f9f9;
}

.tooltip[aria-hidden="true"] {
  visibility: hidden;
  opacity: 0;
  transition: opacity 0.15s, visibility 0.15s;
}

.tooltip[aria-hidden="false"] {
  visibility: visible;
  opacity: 1;
  transition: opacity 0.15s;
}
</style>
