<template>
  <div id="app">
    <v-app id="v-app">
      <router-view/>
    </v-app>
  </div>
</template>


<style lang="scss">
/* default setting */
  * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Montserrat', 'Nanum Gothic'; }
  html, body{ font-size: 10px; }
  a{ display: inline-block; text-decoration: none; color: inherit; }
  button{ background-color: transparent; border: none; cursor: pointer; }
  button:focus{ outline: none; }


  .mw1280{ max-width: 1280px; margin: 0 auto; padding: 80px 40px; }
  .fs16{ font-size: 16px; }
  .fs20{ font-size: 20px; }
  .fs36{ font-size: 36px; }
  .fs60{ font-size: 60px; }

  .text-center{ text-align: center; }
  .uppercase{ text-transform: uppercase; }

  .j-head{ margin-bottom: 40px; font-size: 22px; font-weight: bold; text-transform: uppercase; letter-spacing: 1px; display: inline-block; position: relative; }
  .j-head:before{ content: ""; position: absolute; width: 110%; height: 10px; bottom: 0; left: -5%; background:rgba(27, 184, 80, .5); }
  .j-head span{ position: relative; }
  .j-title{ font-size: 20px; font-weight: bold; }
  .j-text{ font-size: 14px; margin-bottom: 0; }

  .v-application{ line-height: 1.2 !important; }


  @media (max-width: 768px) {
    .mw1280{ padding: 40px 20px; }
    .fs16{ font-size: 12px; }
    .fs20{ font-size: 16px; }
    .fs36{ font-size: 30px; }
    .fs60{ font-size: 50px; }

    .j-head{ font-size: 18px; margin-bottom: 20px; }
    .j-title{ font-size: 16px; }
    .j-text{ font-size: 10px; }
  }

  @media (max-width: 768px){
    .fs16{ font-size: 10px; }
    .fs20{ font-size: 14px; }
    .fs36{ font-size: 26px; }
    .fs60{ font-size: 36px; }

    .j-head{ font-size: 16px; margin-bottom: 20px; }
    .j-title{ font-size: 14px; }
    .j-text{ font-size: 10px; }
  }
</style>
