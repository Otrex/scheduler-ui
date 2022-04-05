<template>
  <div class="">

    <input type="checkbox" id="toggle" class="check-input" v-model="sidebarinput" @change="$emit('checked', sidebarinput)"/>

    <div class="sidebar px-10">
      <div class="py-10">

        <div class="flex items-center justify-between pb-14">
          <div class="flex items-center mx-2">
            <div class="px-2">
              <img src="https://picsum.photos/30/30" class="inline-block h-auto w-auto border-radius-50p bg-#12a8f6 -mr-2" />
            </div>
            <div class="px-2">
              <h1>PJ</h1>
            </div>
          </div>
          <label for="toggle" class="cursor-pointer">
            <svg xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><rect fill="none" height="24" width="24"/><g><polygon points="17.77,3.77 16,2 6,12 16,22 17.77,20.23 9.54,12"/></g></svg>
          </label>
        </div>

        <div class="menu flex flex-col justify-between">
          <ul className="">
            <li class="py-5">
              <nuxt-link to="/" class="flex items-center w-full -mx-2">
                <div class="px-2">
                  <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0z" fill="none"/><path d="M3 13h8V3H3v10zm0 8h8v-6H3v6zm10 0h8V11h-8v10zm0-18v6h8V3h-8z"/></svg>
                </div>
                <span class="px-2 menu-text">Dasboard</span>
              </nuxt-link>
            </li>

            <li class="py-5">
              <nuxt-link to="/" class="flex w-full -mx-2">
                <div class="px-2">
                  <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0z" fill="none"/><path d="M17 4h3v16h-3zM5 14h3v6H5zm6-5h3v11h-3z"/></svg>
                </div>
                <span class="px-2 menu-text">Analytics</span>
              </nuxt-link>
            </li>
            
            <li class="py-5">
              <nuxt-link to="/" class="dashboard-sidebar-links flex items-center w-full -mx-2">
                <div class="px-2">
                  <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0z" fill="none"/><path d="M10 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V8c0-1.1-.9-2-2-2h-8l-2-2z"/></svg>
                </div>
                <span class="px-2 menu-text">Projects</span>
              </nuxt-link>
            </li>

            <li class="py-5">
              <nuxt-link to="/" class="flex items-center w-full -mx-2">
                <div class="px-2">
                  <svg xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><g><rect fill="none" height="24" width="24"/></g><g><g><rect height="2" width="6" x="9" y="1"/><path d="M19.03,7.39l1.42-1.42c-0.43-0.51-0.9-0.99-1.41-1.41l-1.42,1.42C16.07,4.74,14.12,4,12,4c-4.97,0-9,4.03-9,9 c0,4.97,4.02,9,9,9s9-4.03,9-9C21,10.88,20.26,8.93,19.03,7.39z M13,14h-2V8h2V14z"/></g></g></svg>
                </div>
                <span class="px-2 menu-text">Tracking</span>
              </nuxt-link>
            </li>

            <li class="py-5">
              <nuxt-link to="/" class="flex items-center w-full -mx-2">
                <div class="px-2">
                  <svg xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><g><rect fill="none" height="24" width="24"/></g><g><g><g><path d="M12,2C6.5,2,2,6.5,2,12s4.5,10,10,10s10-4.5,10-10S17.5,2,12,2z M16.2,16.2L11,13V7h1.5v5.2l4.5,2.7L16.2,16.2z"/></g></g></g></svg>
                </div>
                <span class="px-2 menu-text">History</span>
              </nuxt-link>
            </li>

            <li class="py-5">
              <nuxt-link to="/" class="flex items-center w-full -mx-2">
                <div class="px-2">
                  <svg xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><g><path d="M0,0h24v24H0V0z" fill="none"/><path d="M19.14,12.94c0.04-0.3,0.06-0.61,0.06-0.94c0-0.32-0.02-0.64-0.07-0.94l2.03-1.58c0.18-0.14,0.23-0.41,0.12-0.61 l-1.92-3.32c-0.12-0.22-0.37-0.29-0.59-0.22l-2.39,0.96c-0.5-0.38-1.03-0.7-1.62-0.94L14.4,2.81c-0.04-0.24-0.24-0.41-0.48-0.41 h-3.84c-0.24,0-0.43,0.17-0.47,0.41L9.25,5.35C8.66,5.59,8.12,5.92,7.63,6.29L5.24,5.33c-0.22-0.08-0.47,0-0.59,0.22L2.74,8.87 C2.62,9.08,2.66,9.34,2.86,9.48l2.03,1.58C4.84,11.36,4.8,11.69,4.8,12s0.02,0.64,0.07,0.94l-2.03,1.58 c-0.18,0.14-0.23,0.41-0.12,0.61l1.92,3.32c0.12,0.22,0.37,0.29,0.59,0.22l2.39-0.96c0.5,0.38,1.03,0.7,1.62,0.94l0.36,2.54 c0.05,0.24,0.24,0.41,0.48,0.41h3.84c0.24,0,0.44-0.17,0.47-0.41l0.36-2.54c0.59-0.24,1.13-0.56,1.62-0.94l2.39,0.96 c0.22,0.08,0.47,0,0.59-0.22l1.92-3.32c0.12-0.22,0.07-0.47-0.12-0.61L19.14,12.94z M12,15.6c-1.98,0-3.6-1.62-3.6-3.6 s1.62-3.6,3.6-3.6s3.6,1.62,3.6,3.6S13.98,15.6,12,15.6z"/></g></svg>
                </div>
                <span class="px-2 menu-text">Settings</span>
              </nuxt-link>
            </li>

            <li class="pt-16">
              <div class="flex items-center justify-between bg-#131e3a-opac border-radius-16px p-5">
                <span class="menu-text">Create <br/> new Task</span>
                <div class="">
                  <div class="bg-#1d5cfc p-3 border-radius-50p">
                    <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#FFFFFF"><path d="M0 0h24v24H0z" fill="none"/><path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/></svg>
                  </div>
                </div>
              </div>
            </li>
          </ul>

          <ul class="">
            <li>
              <div class="flex items-center justify-between">
                <div class="flex user items-center -mx-2">
                  <div class="px-2">
                    <img src="https://picsum.photos/50/50" class="inline-block h-auto w-auto border-radius-50p bg-#12a8f6 -mr-2" />
                  </div>

                  <div class="px-2">
                    <h6>Finna A</h6>
                    <p class="c-#ececec small-p2">finna@iksg.com</p>
                  </div>
                </div>

                <div class="arrow cursor-pointer">
                  <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0z" fill="none"/><path d="M7.41 15.41L12 10.83l4.59 4.58L18 14l-6-6-6 6z"/></svg>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      sidebarinput: null
    }
  },
  emits: ['checked']
}
</script>


<style>
#toggle:checked~.sidebar {
  width: 73px;
  padding-left: 0;
  padding-right: 0;
}

#toggle:checked~.sidebar > div > div > div > div{
  padding-left: 0;
  padding-right: 0;
}

#toggle:checked~.sidebar > div > div{
  justify-content: center;
}

#toggle:checked~.sidebar > div > div > div > div > img{
  display: none
}

#toggle:checked~.sidebar > div > div > div > div > h1{
  font-size: 13px;
}

#toggle:checked~.sidebar > div > .menu > ul > li > a > .menu-text{
  display: none;
}

#toggle:checked~.sidebar > div > .menu > ul > li > a {
  justify-content: center;
}

#toggle:checked~.sidebar > div > .menu > ul > li > div{
  justify-content: center;
}

#toggle:checked~.sidebar > div > .menu > ul > li > div > span{
  display: none;
}

#toggle:checked~.sidebar > div > .menu > ul > li > div > div > div > img {
  display: none;
}

#toggle:checked~.sidebar > div > .menu > ul > li > div > .user {
  display: none;
  margin-left: 0;
  margin-right: 0;
}

#toggle:checked~.sidebar > div > .menu > ul > li > div > .user ~ .arrow{
  margin-top: 40px;
}

</style>