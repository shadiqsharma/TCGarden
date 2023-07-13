<template>
  <div v-if="showModal" class="fixed z-50 inset-0 overflow-y-auto">
    <div class="flex items-center justify-center min-h-screen">
      <div class="bg-white rounded-lg px-4 pt-5 pb-4 text-left overflow-hidden shadow-xl transform transition-all sm:max-w-lg sm:w-full sm:p-6">
        <div class="sm:flex sm:items-start">
          <div class="mx-auto flex-shrink-0 md:w-1/2 rounded-2xl">
            <!-- Image here -->
            <img src="https://res.cloudinary.com/dgsljij3o/image/upload/v1688204965/TC/executive%20queen/photo_2023-06-26_20-56-39_koyzwg.jpg" alt="Promotion Image" class="w-full object-cover rounded-3xl px-1 mr-2">
          </div>
          <div class="mt-3 sm:mt-0 sm:text-left">
            <h3 class="text-lg leading-6 font-medium text-yellow-500" id="modal-title">
              Special Offer!
            </h3>
            <div class="mt-2">
              <p class="text-sm text-gray-500">
                Get a special 20% discount on our premium package when you book today!
              </p>
            </div>
            <div class="mt-5 sm:mt-6">
              <button ref="bookNowButton" class="inline-flex justify-center w-full rounded-md border border-transparent px-4 py-2 bg-indigo-600 text-base font-medium text-white hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500 sm:text-sm">
                Book Now
              </button>
            </div>
          </div>
        </div>
        <div class="mt-5 sm:mt-6">
          <button @click="closeModal" class="text-right text-gray-400 hover:text-gray-500">
            Close
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showModal: true
    }
  },
  methods: {
    closeModal() {
      this.showModal = false;
    },
    handlePromotion() {
      this.closeModal();
      this.$router.push('https://book-directonline.com/properties/tcgardenresortlangkawidirect');
    }
  },
  mounted() {
    this.$refs.bookNowButton.addEventListener('click', () => {
      window.location.href = 'https://book-directonline.com/properties/tcgardenresortlangkawidirect';
    });
  }
}
</script>
