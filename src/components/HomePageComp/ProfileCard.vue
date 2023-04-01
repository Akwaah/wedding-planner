<template>
    <div class="">
        <div class="P400 N700 py-5">Jojo Abbiw</div>
              <div class="P200 N600">
                Aenean imperdiet. Etiam ultricies nisi vel augue. Curabitur ullamcorper ultricies
                nisi. Nam eget dui. Etiam rhoncus. Maecenas tempus, tellus eget condimentum rhoncus,
                sem quam semper libero, sit amet adipiscing sem neque sed ipsum.
              </div>
        <div>
            <!-- <img src="../../assets/2950180.png" alt="" srcset=""> -->
            <Dove/>
        </div>
    </div>
</template>

<script>
import Dove from '../icons/dove.vue';

export default {
    name: "ProfileCard",
    data() {
        return {};
    },
    mounted() {
    },
    methods: {},
    components: { Dove }
};
</script>

<style lang="scss" scoped>

</style>