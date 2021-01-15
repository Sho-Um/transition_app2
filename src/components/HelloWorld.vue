<template>
  <div class="alert alert-primary">
    <h3>{{ title }}</h3>
    <p>{{ message }}</p>
      <div class="list-group">
        <button class="btn btn-primary mb-3"
          v-on:click="doAction1">
        第１位
        </button>
        <transition name="slide-fade">
          <p v-if="flg1" class="trans">嫌われる勇気</p>
        </transition>
        <button class="btn btn-primary mb-3"
          v-on:click="doAction2">
        第２位
        </button>
        <transition name="slide-fade">
          <p v-if="flg2" class="trans">ブループリント</p>
        </transition>
        <button class="btn btn-primary mb-3"
          v-on:click="doAction3">
        第３位
        </button>
        <transition name="slide-fade">
          <p v-if="flg3" class="trans">嫌われる勇気</p>
        </transition>
        <button class="btn btn-primary mb-3"
          v-on:click="doAction4">
        第４位
        </button>
        <transition name="slide-fade">
          <p v-if="flg4" class="trans">ブループリント</p>
        </transition>
        <button class="btn btn-primary mb-3"
          v-on:click="doAction5">
        第５位
        </button>
        <transition name="slide-fade">
          <p v-if="flg5" class="trans">嫌われる勇気</p>
        </transition>
        <button class="btn btn-primary mb-3"
          v-on:click="doAction6">
        第６位
        </button>
        <transition name="slide-fade">
          <p v-if="flg6" class="trans">ブループリント</p>
        </transition>
        <button class="btn btn-primary mb-3"
          v-on:click="doAction7">
        第７位
        </button>
        <transition name="slide-fade">
          <p v-if="flg7" class="trans">嫌われる勇気</p>
        </transition>
        <button class="btn btn-primary mb-3"
          v-on:click="doAction8">
        第８位
        </button>
        <transition name="slide-fade">
          <p v-if="flg8" class="trans">ブループリント</p>
        </transition>
        <button class="btn btn-primary mb-3"
          v-on:click="doAction9">
        第９位
        </button>
        <transition name="slide-fade">
          <p v-if="flg9" class="trans">嫌われる勇気</p>
        </transition>
        <button class="btn btn-primary mb-3"
          v-on:click="doAction10">
        第10位
        </button>
        <transition name="slide-fade">
          <p v-if="flg10" class="trans">ブループリント</p>
        </transition>
      </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: function() {
    return {
      title: '好きな本 BEST10',
      message: '(Readee登録本：388冊)',
      flg1: false,
      flg2: false,
      flg3: false,
      flg4: false,
      flg5: false,
      flg6: false,
      flg7: false,
      flg8: false,
      flg9: false,
      flg10: false,
      btn: 'Hide',
    }
  },
  methods: {
    doAction1() {
      this.flg1 = !this.flg1;
    },
    doAction2() {
      this.flg2 = !this.flg2;
    },
    doAction3() {
      this.flg3 = !this.flg3;
    },
    doAction4() {
      this.flg4 = !this.flg4;
    },
    doAction5() {
      this.flg5 = !this.flg5;
    },
    doAction6() {
      this.flg6 = !this.flg6;
    },
    doAction7() {
      this.flg7 = !this.flg7;
    },
    doAction8() {
      this.flg8 = !this.flg8;
    },
    doAction9() {
      this.flg9 = !this.flg9;
    },
    doAction10() {
      this.flg10 = !this.flg10;
    },
  },
}
</script>

<style>

.trans {
  background-color:lightblue;
  color: black;
  padding: 10px;
  font-size: 20pt;
}

.slide-fade-enter-active {
  transition: all 1.0s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.8s cubic-bezier(1, 0.5, 0.8, 1);
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateX(20px);
  opacity: 0;
}

/* .trans {
  background-color:black;
  color: white;
  padding: 10px;
  font-size: 20pt;
}

.transit-leave-active {
  animation: anim 5.0s;
}

.transit-enter-active {
  animation: anim 5.0s reverse;
}

@keyframes anim {
  0% {
    transform: translateX(0px) translateY(0px) rotateZ(0deg);
    opacity: 1.0;
    background-color: black;
  }
  25% {
    transform: translateX(0px) translateY(0px) rotateZ(0deg);
    opacity: 1.0;
    background-color: black;
    font-size: 30pt;
  }
  50% {
    transform: translateX(0px) translateY(0px) rotateZ(0deg);
    opacity: 1.0;
    background-color: black;
  }
  75% {
    transform: translateX(0px) translateY(0px) rotateZ(0deg);
    opacity: 1.0;
    background-color: black;
  }
  100% {
    transform: translateX(0px) translateY(0px) rotateZ(0deg);
    opacity: 0;
    background-color: black;
    font-size: 10pt;
  }
} */

</style>