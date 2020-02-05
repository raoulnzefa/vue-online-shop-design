<template>
  <div id="app" class="bg-gray-100 h-screen">
    <header class="bg-blue-400 w-full h-104 pt-12 px-56 mb-2">
      <nav class="flex justify-between font-sans mb-12">
        <div class="semi-bold text-lg text-black font-semibold">
          LOGO
        </div>
        <div class="flex">
          <div class="mr-24">
            <a class="semi-bold text-lg text-black font-semibold mr-8 border-b-2 border-transparent hover:border-black" href="#">Discover</a>
            <a class="semi-bold text-lg text-black font-semibold mr-8 border-b-2 border-transparent hover:border-black" href="#">Featured</a>
            <a class="semi-bold text-lg text-black font-semibold border-b-2 border-transparent hover:border-black" href="#">Best Sellers</a>
          </div>
          <div>
            <a href="#" class="mr-3 text-lg text-black font-semibold border-b-2 border-transparent hover:border-black">Sign In</a>
            <a href="#" class="px-8 py-4 rounded bg-gray-900 text-lg text-white font-semibold hover:bg-gray-800">Sign Up</a>
          </div>
        </div>
      </nav>
      <div class="flex shadow-lg">
        <select class="form-select bg-gray-300 font-semibold rounded-r-none w-2/12" name="" id="">
          <option value="everything">Everything</option>
        </select>
        <input type="text" class="form-input w-10/12 px-16 py-4 font-semibold rounded-l-none" placeholder="Search for products & services">
      </div>
    </header>
    <section class="px-56 mb-16">
      <div class="w-full -mt-56">
        <div class="bg-pink-500 flex justify-between px-8 py-8">
          <div>
            <h2 class="font-bold text-white text-2xl">
              Deal of the day
            </h2>
            <p class="font-normal text-white text-lg">
              Hand picked by allinite staff
            </p>
          </div>
          <div class="pt-2">
            <button class="px-2 py-3 bg-white rounded border-2 border-black text-lg font-semibold hover:bg-black hover:text-white">
              Discover the best products
            </button>
          </div>
        </div>
        <div>
          <img class="w-full" src="./assets/banner.png" alt="">
        </div>
      </div>
    </section>
    <main class="px-56 bg-gray-100 pb-56">
      <div class="py-4 border-b-2 border-gray-400 mb-8">
        <a class="semi-bold text-lg text-black font-semibold mr-8 border-b-2 border-transparent hover:border-black" href="#">Featured</a>
        <a class="semi-bold text-lg text-black font-semibold mr-8 border-b-2 border-transparent hover:border-black" href="#">Best Sellers</a>
        <a class="semi-bold text-lg text-black font-semibold mr-8 border-b-2 border-transparent hover:border-black" href="#">Home & Garden</a>
        <a class="semi-bold text-lg text-black font-semibold mr-8 border-b-2 border-transparent hover:border-black" href="#">Beauty & Fashion</a>
        <a class="semi-bold text-lg text-black font-semibold mr-8 border-b-2 border-transparent hover:border-black" href="#">Tech & Gadgets</a>
        <a class="semi-bold text-lg text-black font-semibold border-b-2 border-transparent hover:border-black" href="#">Discover Products</a>
      </div>
      <div class="bg-gray-100">
        <div class="mb-16">
          <span class="bg-pink-500 pl-8 pr-12 py-2 capitalize font-medium text-white">featured</span>
        </div>
        <div class="flex justify-between">
          <div v-for="(i,key) in 3" :key="key" class="relative w-1/3 border" :class="{'ml-4': key>0}">
            <span class="bg-orange-400 font-black text-4xl text-white px-1 absolute -mt-6 ml-2">
              $99.99
            </span>
            <div class="bg-gray-400 h-40">
            </div>
            <div>
              <p class="px-2 text-xl font-bold text-black mb-6">
                JBL Noise Cancelling Headphones 
              </p>
              <div class="px-2 flex flex-start mb-2">
                <span class="bg-blue-200 rounded-full p-2 mr-4">
                  <svg width="20" height="20" class="text-blue-900 fill-current" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                    <path d="M10 20C7.34784 20 4.8043 18.9464 2.92893 17.0711C1.05357 15.1957 0 12.6522 0 10C0 7.34784 1.05357 4.8043 2.92893 2.92893C4.8043 1.05357 7.34784 0 10 0C12.6522 0 15.1957 1.05357 17.0711 2.92893C18.9464 4.8043 20 7.34784 20 10C20 12.6522 18.9464 15.1957 17.0711 17.0711C15.1957 18.9464 12.6522 20 10 20ZM10 18C12.1217 18 14.1566 17.1571 15.6569 15.6569C17.1571 14.1566 18 12.1217 18 10C18 7.87827 17.1571 5.84344 15.6569 4.34315C14.1566 2.84285 12.1217 2 10 2C7.87827 2 5.84344 2.84285 4.34315 4.34315C2.84285 5.84344 2 7.87827 2 10C2 12.1217 2.84285 14.1566 4.34315 15.6569C5.84344 17.1571 7.87827 18 10 18ZM6.46 13.54C6.2717 13.3517 6.16591 13.0963 6.16591 12.83C6.16591 12.5637 6.2717 12.3083 6.46 12.12C6.6483 11.9317 6.9037 11.8259 7.17 11.8259C7.4363 11.8259 7.6917 11.9317 7.88 12.12C8.4425 12.6818 9.205 12.9974 10 12.9974C10.795 12.9974 11.5575 12.6818 12.12 12.12C12.3083 11.9317 12.5637 11.8259 12.83 11.8259C13.0963 11.8259 13.3517 11.9317 13.54 12.12C13.7283 12.3083 13.8341 12.5637 13.8341 12.83C13.8341 13.0963 13.7283 13.3517 13.54 13.54C13.0755 14.0056 12.5238 14.3751 11.9163 14.6271C11.3089 14.8792 10.6577 15.0089 10 15.0089C9.34233 15.0089 8.69112 14.8792 8.08366 14.6271C7.47621 14.3751 6.92446 14.0056 6.46 13.54ZM7 9C6.73478 9 6.48043 8.89464 6.29289 8.70711C6.10536 8.51957 6 8.26522 6 8C6 7.73478 6.10536 7.48043 6.29289 7.29289C6.48043 7.10536 6.73478 7 7 7C7.26522 7 7.51957 7.10536 7.70711 7.29289C7.89464 7.48043 8 7.73478 8 8C8 8.26522 7.89464 8.51957 7.70711 8.70711C7.51957 8.89464 7.26522 9 7 9ZM13 9C12.7348 9 12.4804 8.89464 12.2929 8.70711C12.1054 8.51957 12 8.26522 12 8C12 7.73478 12.1054 7.48043 12.2929 7.29289C12.4804 7.10536 12.7348 7 13 7C13.2652 7 13.5196 7.10536 13.7071 7.29289C13.8946 7.48043 14 7.73478 14 8C14 8.26522 13.8946 8.51957 13.7071 8.70711C13.5196 8.89464 13.2652 9 13 9Z"/>
                  </svg>
                </span>
                <span class="mt-2 text-gray-600">Blessed T Mahuni</span>
              </div>
              <div class="px-2 mb-2 flex flex-start">
                <span class="flex mr-4">
                  <svg v-for="(i,key) in 5" :key="key" class="text-gray-500 fill-current" width="23" height="22" viewBox="0 0 23 22" xmlns="http://www.w3.org/2000/svg">
                    <path d="M6.1 20.98C5.9344 21.0671 5.74768 21.106 5.56108 21.0922C5.37448 21.0785 5.19548 21.0126 5.04443 20.9022C4.89338 20.7918 4.77634 20.6412 4.70662 20.4676C4.63689 20.294 4.61728 20.1042 4.65 19.92L5.68 13.89L1.3 9.63002C1.165 9.49957 1.06944 9.33375 1.02426 9.15154C0.979084 8.96932 0.986109 8.77807 1.04454 8.59966C1.10296 8.42125 1.21043 8.26289 1.35464 8.1427C1.49885 8.02251 1.67399 7.94534 1.86 7.92002L7.91 7.04002L10.61 1.56002C10.6919 1.39095 10.8197 1.24836 10.9789 1.14859C11.1381 1.04883 11.3221 0.995911 11.51 0.995911C11.6979 0.995911 11.8819 1.04883 12.0411 1.14859C12.2003 1.24836 12.3281 1.39095 12.41 1.56002L15.11 7.04002L21.17 7.92002C21.3532 7.94828 21.5248 8.02687 21.6659 8.14703C21.807 8.26719 21.9119 8.42419 21.969 8.60051C22.026 8.77682 22.0329 8.96552 21.989 9.14555C21.945 9.32557 21.8519 9.48984 21.72 9.62002L17.34 13.89L18.38 19.92C18.4141 20.1056 18.395 20.297 18.325 20.4722C18.2549 20.6474 18.1367 20.7992 17.984 20.9101C17.8313 21.0209 17.6504 21.0863 17.4621 21.0987C17.2738 21.1111 17.0859 21.0699 16.92 20.98L11.52 18.13L6.1 20.98ZM11.05 16.11C11.1934 16.0347 11.353 15.9953 11.515 15.9953C11.677 15.9953 11.8366 16.0347 11.98 16.11L16.06 18.26L15.28 13.71C15.2538 13.5508 15.2664 13.3876 15.3169 13.2344C15.3674 13.0812 15.4543 12.9424 15.57 12.83L18.87 9.61002L14.31 8.94002C14.149 8.91851 13.9956 8.8581 13.8632 8.76401C13.7308 8.66992 13.6233 8.54499 13.55 8.40002L11.51 4.26002L9.47 8.40002C9.39765 8.54372 9.29169 8.66785 9.16113 8.76186C9.03056 8.85587 8.87924 8.91698 8.72 8.94002L4.15 9.61002L7.45 12.83C7.56753 12.9414 7.65624 13.0797 7.70849 13.233C7.76075 13.3863 7.77499 13.55 7.75 13.71L6.96 18.26L11.05 16.11Z"/>
                  </svg>
                </span>
                <span class="text-gray-600">
                  2.5k Ratings
                </span>
              </div>
              <div class="bg-blue-200 p-2">
                <button class="text-white flex bg-blue-600 py-2 px-16 rounded hover:bg-blue-500 mx-auto">
                  <svg width="22" height="20" class="fill-current mr-4" viewBox="0 0 22 20" xmlns="http://www.w3.org/2000/svg">
                    <path d="M16 14C16.6367 14.0003 17.2569 14.2033 17.7707 14.5794C18.2844 14.9556 18.6652 15.4855 18.8578 16.0924C19.0505 16.6993 19.045 17.3518 18.8422 17.9554C18.6394 18.559 18.2498 19.0824 17.7298 19.4499C17.2098 19.8174 16.5864 20.0099 15.9497 19.9996C15.313 19.9893 14.6961 19.7766 14.1883 19.3924C13.6805 19.0082 13.3082 18.4724 13.1251 17.8625C12.942 17.2527 12.9577 16.6003 13.17 16H8.82999C8.99134 16.4567 9.0397 16.9457 8.97093 17.4252C8.90216 17.9047 8.71831 18.3604 8.43509 18.7534C8.15187 19.1463 7.7777 19.4649 7.34458 19.6818C6.91146 19.8987 6.43226 20.0075 5.94794 19.9988C5.46363 19.9902 4.9886 19.8645 4.56347 19.6323C4.13834 19.4001 3.77574 19.0685 3.50668 18.6657C3.23762 18.2629 3.0701 17.8009 3.01843 17.3193C2.96676 16.8377 3.03249 16.3507 3.20999 15.9C2.50381 15.713 1.89011 15.2748 1.48403 14.6676C1.07795 14.0604 0.907379 13.3258 1.00433 12.6018C1.10128 11.8777 1.45908 11.2139 2.01061 10.7349C2.56214 10.2559 3.2695 9.9946 3.99999 10V2H1.99999C1.73477 2 1.48042 1.89464 1.29288 1.70711C1.10534 1.51957 0.999986 1.26522 0.999986 1C0.999986 0.734784 1.10534 0.48043 1.29288 0.292893C1.48042 0.105357 1.73477 0 1.99999 0H4.99999C5.2652 0 5.51956 0.105357 5.70709 0.292893C5.89463 0.48043 5.99999 0.734784 5.99999 1V2H20C20.1713 1.9988 20.34 2.04164 20.49 2.12439C20.64 2.20715 20.7663 2.32706 20.8566 2.47261C20.947 2.61817 20.9984 2.78449 21.006 2.95564C21.0136 3.12679 20.9771 3.29701 20.9 3.45L16.9 11.45C16.8161 11.6164 16.6874 11.7561 16.5284 11.8533C16.3694 11.9505 16.1864 12.0013 16 12H3.99999C3.73477 12 3.48042 12.1054 3.29288 12.2929C3.10534 12.4804 2.99999 12.7348 2.99999 13C2.99999 13.2652 3.10534 13.5196 3.29288 13.7071C3.48042 13.8946 3.73477 14 3.99999 14H16ZM5.99999 10H15.38L18.38 4H5.99999V10ZM5.99999 18C6.2652 18 6.51956 17.8946 6.70709 17.7071C6.89463 17.5196 6.99999 17.2652 6.99999 17C6.99999 16.7348 6.89463 16.4804 6.70709 16.2929C6.51956 16.1054 6.2652 16 5.99999 16C5.73477 16 5.48042 16.1054 5.29288 16.2929C5.10534 16.4804 4.99999 16.7348 4.99999 17C4.99999 17.2652 5.10534 17.5196 5.29288 17.7071C5.48042 17.8946 5.73477 18 5.99999 18ZM16 18C16.2652 18 16.5196 17.8946 16.7071 17.7071C16.8946 17.5196 17 17.2652 17 17C17 16.7348 16.8946 16.4804 16.7071 16.2929C16.5196 16.1054 16.2652 16 16 16C15.7348 16 15.4804 16.1054 15.2929 16.2929C15.1053 16.4804 15 16.7348 15 17C15 17.2652 15.1053 17.5196 15.2929 17.7071C15.4804 17.8946 15.7348 18 16 18Z"/>
                  </svg>
                  <span>Add To Cart</span>
                </button>
              </div>
            </div>

          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>


export default {
  name: 'app',
  
}
</script>

<style src='./assets/css/tailwind.css'>

</style>
