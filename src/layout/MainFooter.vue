<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <div class="row">
    <div class="col">
      <h5>Location :</h5>
      สาขาวิชาวิทยาการคอมพิวเตอร์ คณะวิทยาศาสตร์ มหาวิทยาลัยแม่โจ้
      63 หมู่ 4 ต.หนองหาร อ.สันทราย จ.เชียงใหม่ 50290
      {{Map}}
    </div>
    <div class="col">
      Contact : 
    </div>
    <div class="col">
      Logo
    </div>
  </div>
  <hr>
  
      <div class="copyright container text-center">
        &copy; {{ year }} All Rights Reserved.
        <p>Development & Design by HOP Teams | CSMJU 24</p>

      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
