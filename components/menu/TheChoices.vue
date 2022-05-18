<template>
    <v-item-group active-class="primary">
        <!-- <v-container> -->
        <v-row>
            <v-col
            v-for="item in languages"
            :key="item.id"
            >
            <v-item v-slot="{ active, toggle }">
                <v-card
                    class="d-flex align-center"
                    style="backgroundColor: #424242"
                    elevation="10"
                    height="60"
                    width="200"
                    @click="toggle"
                >
                    <v-card-text class="text-h4 flex-grow-1 text-center">
                        {{ item.language }}
                    </v-card-text>
                    <v-scroll-y-transition>
                        <div
                            v-if="active"
                            class="text-h4 flex-grow-1 text-center"
                        >
                        </div>
                    </v-scroll-y-transition>
                </v-card>
            </v-item>
            </v-col>
        </v-row>
        <!-- </v-container> -->
    </v-item-group>

</template>

<script>
export default {
    data() {
        return {
            languages: [
                { id: 1, language: "Spanish" },
                { id: 2, language: "German" },
                { id: 3, language: "Dutch" }
            ]
        }
    }
}
</script>

<style>

</style>