<i18n>
{
  "en": {
    "title": "Holistic Therapy",
    "design": {
      "subtitle": "Reiki",
      "description": "Lorem Ipsum",
      "cta": "Lorem Ipsum"
    },
    "development": {
      "subtitle": "Natural Medicine",
      "description": "Lorem Ipsum",
      "cta": "Lorem Ipsum"
    },
    "marketing": {
      "subtitle": "Meditation Groups",
      "description": "Lorem Ipsum",
      "cta": "Lorem Ipsum"
    }
  },
  "es": {
    "title": "Terapias Holisticas",
    "design": {
      "subtitle": "Reiki.",
      "description": "Lorem Ipsum",
      "cta": "Lorem Ipsum"
    },
    "development": {
      "subtitle": "Medicina natural",
      "description": "Lorem Ipsum",
      "cta": "Lorem Ipsum"
    },
    "marketing": {
      "subtitle": "Grupos de Meditacion",
      "description": "Lorem Ipsum",
      "cta": "Lorem Ipsum"
    }
  }
}
</i18n>

<template>
  <div
    class="
      relative
      bg-purple-500
      pt-16
      pb-20
      px-4
      sm:px-6
      lg:pt-24
      lg:pb-28
      lg:px-8
    "
  >
    <div class="relative max-w-7xl mx-auto">
      <div class="text-center content-center py-20">
        <Buda class="fadeOut scrolldown"/>
        <h2
          class="
            fadeIn
            text-4xl
            tracking-tight
            font-extrabold
            text-gray-900
            sm:text-7xl
          "
        >
          {{ $t('title') }}
        </h2>
        <p class="downarrows pt-32 text-lg font-semibold text-gray-900">
          scroll down
        </p>
        <p class="downarrows pt-12 text-xl font-semibold text-gray-900">↓</p>
      </div>
      <div
        class="-mt-32 max-w-lg mx-auto grid gap-5 lg:grid-cols-3 lg:max-w-none"
      >
        <div class="grow fadeIn flex flex-col rounded-lg overflow-hidden">
          <div class="flex-1 p-6 flex flex-col justify-between">
            <div class="flex-1">
              <div class="block mt-2">
                <p class="text-xl text-center font-semibold text-gray-900">
                  {{ $t('design.subtitle') }}
                </p>
                <p class="mt-3 text-center text-base text-gray-500">
                  {{ $t('design.description') }}
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="grow fadeIn flex flex-col rounded-lg overflow-hidden">
          <div class="flex-1 p-6 flex flex-col justify-between">
            <div class="flex-1">
              <div class="block mt-2">
                <p class="text-xl text-center font-semibold text-gray-900">
                  {{ $t('development.subtitle') }}
                </p>
                <p class="mt-3 text-center text-base text-gray-500">
                  {{ $t('development.description') }}
                </p>
              </div>
            </div>
            <!-- <div class="mt-6 flex items-center">
              <nuxt-link
                :to="localePath('development')"
                class="
                  mt-8
                  block
                  w-full
                  bg-gray-900
                  border border-gray-800
                  rounded-md
                  py-2
                  text-sm
                  font-semibold
                  text-white text-center
                  hover:bg-gray-700
                "
              >
                {{ $t('development.cta') }}
              </nuxt-link>
            </div> -->
          </div>
        </div>
        <div class="grow fadeIn flex flex-col rounded-lg overflow-hidden">
          <div class="flex-1 p-6 flex flex-col justify-between">
            <div class="flex-1">
              <div class="block mt-2">
                <p class="text-xl text-center font-semibold text-gray-900">
                  {{ $t('marketing.subtitle') }}
                </p>
                <p class="mt-3 text-center text-base text-gray-500">
                  {{ $t('marketing.description') }}
                </p>
              </div>
            </div>
            <!-- <div class="mt-6 flex items-center">
              <nuxt-link
                :to="localePath('marketing')"
                class="
                  mt-8
                  block
                  w-full
                  bg-gray-800
                  border border-gray-900
                  rounded-md
                  py-2
                  text-sm
                  font-semibold
                  text-white text-center
                  hover:bg-gray-700
                "
              >
                {{ $t('marketing.cta') }}
              </nuxt-link>
            </div> -->
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- <main class="bg-yellow-500 pt-16 px-auto max-w-7xl px-4 sm:pt-24">
    <div class="text-center">
      <h1
        class="
          text-4xl
          tracking-tight
          font-extrabold
          text-gray-900
          sm:text-5xl
          md:text-6xl
        "
      >
        <span class="block xl:inline">Scale with us.</span>
      </h1>
      <p
        class="
          mt-3
          max-w-md
          mx-auto
          text-base text-gray-900
          sm:text-lg
          md:mt-5
          md:text-xl
          md:max-w-3xl
        "
      >
        You have the idea, we have the people to build it.
      </p>
      <div
        class="mt-5 max-w-md mx-auto sm:flex sm:justify-center md:mt-8"
      ></div>
    </div>
  </main> -->
</template>

<script>
import lax from 'lax.js'

export default {
  mounted() {
    lax.init()
    lax.addDriver('scrollY', function () {
      return window.scrollY
    })
    lax.addElements('.fadeIn', {
      scrollY: {
        opacity: [
          [0, 100],
          [0, 1],
        ],
      },
    })
    lax.addElements('.scrolldown', {
      scrollY: {
        'letter-spacing': [
          [0, 'screenHeight*0.75'],
          [0, 150],
          {
            cssUnit: 'px',
          },
        ],
        opacity: [
          [0, 100],
          [1, 0],
        ],
        translateX: [
          [0, 'screenHeight'],
          [0, 80],
        ],
      },
    })
    lax.addElements('.fadeOut', {
      scrollY: {
        opacity: [
          [0, 100],
          [1, 0],
        ],
      },
    })
    lax.addElements('.letter-x', {
      scrollY: {
        translateY: [
          [-400, 0],
          [100, 0],
        ],
        translateX: [
          [220, 'screenHeight'],
          [0, 400],
        ],
        opacity: [
          [0, 100],
          [0, 1],
        ],
      },
    })
    lax.addElements('.letter-a', {
      scrollY: {
        translateY: [
          [-400, 0],
          [200, 0],
        ],
        translateX: [
          [220, 'screenHeight'],
          [0, -400],
        ],
        opacity: [
          [0, 100],
          [0, 1],
        ],
      },
    })
    lax.addElements('.downarrows', {
      scrollY: {
        translateY: [
          [0, 75],
          [0, 200],
        ],
        opacity: [
          [0, 100],
          [1, 0],
        ],
      },
    })
    lax.addElements('.grow', {
      scrollY: {
        scale: [
          [30, 100],
          [0.3, 1],
        ],
      },
    })
  },
  beforeUnmount() {
    lax.removeElements(
      '.fadeIn',
      '.grow',
      '.downarrows',
      '.letter-a',
      '.letter-x',
      '.fadeOut',
      '.scrolldown'
    )
  },
}
</script>

<style>
body{font:normal normal 14px/19px Arial,sans-serif;letter-spacing:1px;margin:0;background:#FFFFFF}
::-moz-selection{background:#F37043;color:#FFFFFF}
::selection{background:#F37043;color:#FFFFFF}
.clearfix{display:inline-block}
.clearfix::after{content:"";visibility:hidden;display:inline-block;font-size:0;clear:both;height:0}
.tekst{color:#363635;font-family:Arial,sans-serif;text-transform:uppercase;font-size:14px;line-height:28px;font-weight:bold;display:block;letter-spacing:2px;max-width:100%;text-align:center;position:absolute;bottom:20px;left:30px;z-index:99}
a{color:#F37043;text-decoration:none;cursor:pointer}
a:hover{text-decoration:underline}
.outer{display:table;margin:0 auto;height:100%}
.middle{display:table-cell;vertical-align:middle}
.main{position:relative;height:190px;margin:18px}
@media (max-width:550px){.main{-webkit-transform:scale(0.75);transform:scale(0.75)}}
@media (max-width:440px){.main{-webkit-transform:scale(0.5);transform:scale(0.5)}}
.buddha{position:relative;width:128px;height:190px;-webkit-animation:animUpDown 3s ease-in-out infinite;animation:animUpDown 3s ease-in-out infinite}
.buddha .legs{position:absolute;bottom:0;left:0;width:128px;height:50px;border-radius:50px;background:#F37043}
.buddha .tail{position:absolute;bottom:10px;left:15px;width:98px;height:82px;border-radius:38px;background:#F37043}
.buddha .head{position:absolute;top:0px;left:2px;width:124px;height:124px;border-radius:124px;background:#F2BC9B}
.buddha .ears{position:absolute;bottom:28px;width:28px;height:28px;border-radius:28px;background:#F2BC9B}
.buddha .ears.left{left:-10px}
.buddha .ears.right{right:-10px}
.buddha .hand{position:absolute;bottom:25px;left:50%;width:34px;height:34px;border-radius:34px;background:#F2BC9B;-webkit-transform:translateX(-50%);transform:translateX(-50%)}
.buddha .mouth{position:absolute;bottom:25px;left:50%;width:16px;height:6px;margin-left:-12px;border:5px solid #F05978;border-top:0;border-radius:0 0 20px 20px / 0 0 16px 16px}
.buddha .circle{position:absolute;top:45px;left:50%;width:12px;height:12px;border-radius:12px;background:#F05978;-webkit-transform:translateX(-50%);transform:translateX(-50%)}
.buddha .eye{position:absolute;bottom:50px;width:10px;height:5px;border:6px solid #363635;border-bottom:0;border-radius:10px 10px 0 0 / 10px 10px 0 0}
.buddha .eye.left{left:25px}
.buddha .eye.right{right:25px}
.shadow{position:absolute;bottom:-40px;display:block;width:128px;height:50px;background:rgba(0,0,0,0.2);border-radius:50%;-webkit-animation:animShadow 3s ease-in-out infinite;animation:animShadow 3s ease-in-out infinite}
@-webkit-keyframes animShadow{0%,100%{-webkit-transform:scale(1) rotateX(100deg);transform:scale(1) rotateX(100deg)}50%{-webkit-transform:scale(0.7) rotateX(100deg);transform:scale(0.7) rotateX(100deg)}}
@keyframes animShadow{0%,100%{-webkit-transform:scale(1) rotateX(100deg);transform:scale(1) rotateX(100deg)}50%{-webkit-transform:scale(0.7) rotateX(100deg);transform:scale(0.7) rotateX(100deg)}}
@-webkit-keyframes animUpDown{0%,100%{-webkit-transform:translateY(0);transform:translateY(0)}50%{-webkit-transform:translateY(-25px);transform:translateY(-25px)}}
@keyframes animUpDown{0%,100%{-webkit-transform:translateY(0);transform:translateY(0)}50%{-webkit-transform:translateY(-25px);transform:translateY(-25px)}}
.main:hover .buddha .head{-webkit-animation:animTopBottom 0.25s infinite;animation:animTopBottom 0.25s infinite}
@-webkit-keyframes animTopBottom{0%,100%{-webkit-transform:translateY(0);transform:translateY(0)}50%{-webkit-transform:translateY(-5px);transform:translateY(-5px)}}
@keyframes animTopBottom{0%,100%{-webkit-transform:translateY(0);transform:translateY(0)}50%{-webkit-transform:translateY(-5px);transform:translateY(-5px)}}

</style>