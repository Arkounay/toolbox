<template>
    <div>
        <div class="bg-grey">
            <div class="input-validate">
                <i class="icon icon-lock"></i>
                <input type="text" id="text" name="text">
                <label for="text">Input text</label>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @import 'src/scss/utils/variables';
    @import 'src/scss/utils/reboot';
    @import 'src/scss/utils/resets';
    @import 'src/scss/utils/easing';
    @import 'src/scss/utils/mixins';
    @import 'src/scss/typography/iconfont';
    @import 'src/scss/components/input/material';

    .bg-grey {
        background-color: $color-grey;
        padding: 15px;
    }
</style>

<script>
  import {MaterialInput} from '../../../../src/js/forms/MaterialInput';

  export default {
    mounted() {
      new MaterialInput({
        element: document.querySelectorAll('.input-validate')
      });
    }
  }
</script>