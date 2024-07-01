<script setup>
import contributionShape_1 from "/assets/img/images/contribution_shape01.png";
import contributionShape_2 from "/assets/img/images/contribution_shape02.png";
</script>

<template>
  <section id="contribution" class="contribution-area pt-130 pb-130">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-10">
          <div class="contribution-title">
            <h2 class="title">
              <span>$45,256,432</span><br />
              Total Bank
            </h2>
          </div>
          <div class="contribution-title">
            <h4 class="title">
              <span>$45,256,432</span><br />
              Contribution Receive
            </h4>
          </div>
          <div class="contribution-title">
            <h5 class="title">
              <span>$45,256,432</span><br />
              Cashout Send
            </h5>
          </div>
        </div>
      </div>
    </div>
    <div class="contribution-shape-wrap">
      <img :src="contributionShape_1" alt="" class="alltuchtopdown" />
      <img :src="contributionShape_2" alt="" class="leftToRight" />
    </div>
  </section>
</template>
