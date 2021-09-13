<i18n>
  {
    "en": {
      "copyright": "All rights reserved",
      "tagline": "Holistic Therapy",
      "links": {
        "services": {
          "title": "Services",
          "design": "Design",
          "development": "Development",
          "marketing": "Marketing"
        },
        "legal": {
          "title": "Legal",
          "privacy": "Privacy",
          "terms": "Terms and Conditions",
          "data": "Data Compliance"
        },
        "company": {
          "title": "Company",
          "about": "About Us",
          "work": "Our Work",
          "news": "News",
          "intern": "Internships",
          "jobs": "Jobs",
          "partners": "Partners"
        }
      },
      "ctas": {
        "contact": "Contact Us",
        "meet": "Meet with Us"
      }
    },
    "es": {
      "copyright": "Todos los derechos reservados",
      "tagline": "Terapias Holisticas",
      "links": {
        "services": {
          "title": "Servicios",
          "design": "Diseño",
          "development": "Desarrollo",
          "marketing": "Marketing"
        },
        "legal": {
          "title": "Legal",
          "privacy": "Privacidad",
          "terms": "Términos y condiciones",
          "data": "Data Compliance"
        },
        "company": {
          "title": "Compañía",
          "about": "Sobre nosotros",
          "work": "Nuestro Trabajo",
          "news": "Novedades",
          "intern": "Pasantías",
          "jobs": "Llamados laborales",
          "partners": "Asociaciones"
        }
      },
      "ctas": {
        "contact": "Contáctanos",
        "meet": "Tengamos una reunión"
      }
    }
  }

</i18n>
<template>
  <!-- This example requires Tailwind CSS v2.0+ -->
  <footer class="bg-purple-500" aria-labelledby="footerHeading">
    <h2 id="footerHeading" class="sr-only">Footer</h2>
    <div class="max-w-7xl mx-auto py-12 px-4 sm:px-6 lg:py-16 lg:px-8">
      <div class="xl:grid xl:grid-cols-3 xl:gap-8">
        <div class="space-y-8 xl:col-span-1">
          <div class="flex justify-start lg:w-0 lg:flex-1">
            <nuxt-link
              :to="localePath('/')"
              class="text-xl text-gray-800 hover:text-gray-800 font-bold mb-1"
            >
              Reiki
            </nuxt-link>
          </div>
          <p class="text-gray-800 text-base font-bold">{{ $t('tagline') }}</p>
          <div class="flex space-x-6">
            <a
              href="https://www.facebook.com/zaelotcom"
              target="__blank"
              rel="roreferrer noopener"
              class="text-gray-800 hover:text-gray-800"
            >
              <span class="sr-only">Facebook</span>
              <svg
                class="h-6 w-6"
                fill="currentColor"
                viewBox="0 0 24 24"
                aria-hidden="true"
              >
                <path
                  fill-rule="evenodd"
                  d="M22 12c0-5.523-4.477-10-10-10S2 6.477 2 12c0 4.991 3.657 9.128 8.438 9.878v-6.987h-2.54V12h2.54V9.797c0-2.506 1.492-3.89 3.777-3.89 1.094 0 2.238.195 2.238.195v2.46h-1.26c-1.243 0-1.63.771-1.63 1.562V12h2.773l-.443 2.89h-2.33v6.988C18.343 21.128 22 16.991 22 12z"
                  clip-rule="evenodd"
                />
              </svg>
            </a>

            <a
              rel="noopener noreferrer"
              href="https://www.instagram.com/zaelotinc/"
              class="text-gray-800 hover:text-gray-800"
            >
              <span class="sr-only">Instagram</span>
              <svg
                class="h-6 w-6"
                fill="currentColor"
                viewBox="0 0 24 24"
                aria-hidden="true"
              >
                <path
                  fill-rule="evenodd"
                  d="M12.315 2c2.43 0 2.784.013 3.808.06 1.064.049 1.791.218 2.427.465a4.902 4.902 0 011.772 1.153 4.902 4.902 0 011.153 1.772c.247.636.416 1.363.465 2.427.048 1.067.06 1.407.06 4.123v.08c0 2.643-.012 2.987-.06 4.043-.049 1.064-.218 1.791-.465 2.427a4.902 4.902 0 01-1.153 1.772 4.902 4.902 0 01-1.772 1.153c-.636.247-1.363.416-2.427.465-1.067.048-1.407.06-4.123.06h-.08c-2.643 0-2.987-.012-4.043-.06-1.064-.049-1.791-.218-2.427-.465a4.902 4.902 0 01-1.772-1.153 4.902 4.902 0 01-1.153-1.772c-.247-.636-.416-1.363-.465-2.427-.047-1.024-.06-1.379-.06-3.808v-.63c0-2.43.013-2.784.06-3.808.049-1.064.218-1.791.465-2.427a4.902 4.902 0 011.153-1.772A4.902 4.902 0 015.45 2.525c.636-.247 1.363-.416 2.427-.465C8.901 2.013 9.256 2 11.685 2h.63zm-.081 1.802h-.468c-2.456 0-2.784.011-3.807.058-.975.045-1.504.207-1.857.344-.467.182-.8.398-1.15.748-.35.35-.566.683-.748 1.15-.137.353-.3.882-.344 1.857-.047 1.023-.058 1.351-.058 3.807v.468c0 2.456.011 2.784.058 3.807.045.975.207 1.504.344 1.857.182.466.399.8.748 1.15.35.35.683.566 1.15.748.353.137.882.3 1.857.344 1.054.048 1.37.058 4.041.058h.08c2.597 0 2.917-.01 3.96-.058.976-.045 1.505-.207 1.858-.344.466-.182.8-.398 1.15-.748.35-.35.566-.683.748-1.15.137-.353.3-.882.344-1.857.048-1.055.058-1.37.058-4.041v-.08c0-2.597-.01-2.917-.058-3.96-.045-.976-.207-1.505-.344-1.858a3.097 3.097 0 00-.748-1.15 3.098 3.098 0 00-1.15-.748c-.353-.137-.882-.3-1.857-.344-1.023-.047-1.351-.058-3.807-.058zM12 6.865a5.135 5.135 0 110 10.27 5.135 5.135 0 010-10.27zm0 1.802a3.333 3.333 0 100 6.666 3.333 3.333 0 000-6.666zm5.338-3.205a1.2 1.2 0 110 2.4 1.2 1.2 0 010-2.4z"
                  clip-rule="evenodd"
                />
              </svg>
            </a>

            <a
              rel="noopener noreferrer"
              href="https://twitter.com/ZaelotInc"
              class="text-gray-800 hover:text-gray-800"
            >
              <span class="sr-only">Twitter</span>
              <svg
                class="h-6 w-6"
                fill="currentColor"
                viewBox="0 0 24 24"
                aria-hidden="true"
              >
                <path
                  d="M8.29 20.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0022 5.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.072 4.072 0 012.8 9.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 012 18.407a11.616 11.616 0 006.29 1.84"
                />
              </svg>
            </a>

            <a
              rel="noopener noreferrer"
              href="https://github.com/Zaelot-Inc"
              class="text-gray-800 hover:text-gray-800"
            >
              <span class="sr-only">GitHub</span>
              <svg
                class="h-6 w-6"
                fill="currentColor"
                viewBox="0 0 24 24"
                aria-hidden="true"
              >
                <path
                  fill-rule="evenodd"
                  d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z"
                  clip-rule="evenodd"
                />
              </svg>
            </a>

            <a
              rel="noopener noreferrer"
              href="https://medium.com/zaelot"
              class="text-gray-800 hover:text-gray-800"
            >
              <span class="sr-only">Medium</span>

              <svg
                class="h-6 w-6"
                width="80px"
                height="46px"
                viewBox="0 0 80 46"
                version="1.1"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
              >
                <g
                  id="Page-1"
                  stroke="none"
                  stroke-width="1"
                  fill="none"
                  fill-rule="evenodd"
                >
                  <g
                    id="Medium-Logo-Black-RGB_300x80"
                    transform="translate(0.000000, 0.000000)"
                    fill="#1f2937"
                    fill-rule="nonzero"
                  >
                    <path
                      id="Path"
                      d="M45,23.1 C45,35.6 34.9,45.7 22.5,45.7 C10.1,45.7 0,35.7 0,23.1 C0,10.5 10.1,0.5 22.5,0.5 C34.9,0.5 45,10.6 45,23.1"
                    ></path>
                    <path
                      id="Path"
                      d="M69.7,23.1 C69.7,34.9 64.7,44.4 58.5,44.4 C52.3,44.4 47.3,34.9 47.3,23.1 C47.3,11.3 52.3,1.8 58.5,1.8 C64.6,1.8 69.7,11.4 69.7,23.1"
                    ></path>
                    <path
                      id="Path"
                      d="M79.7,23.1 C79.7,33.6 77.9,42.2 75.7,42.2 C73.5,42.2 71.7,33.6 71.7,23.1 C71.7,12.6 73.5,4 75.7,4 C78,4 79.7,12.6 79.7,23.1"
                    ></path>
                  </g>
                </g>
              </svg>
            </a>
          </div>
        </div>
      </div>
      <div class="mt-12 border-t border-gray-900 pt-8">
        <p class="text-xs text-gray-800 xl:text-center">
          &copy; {{ currentYear }} {{ $t('copyright') }}.
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  computed: {
    currentYear() {
      return new Date().getFullYear()
    },
  },
}
</script>
