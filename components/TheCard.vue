<template>
    <v-container>
        <v-row justify="center" class="my-12" >
            <v-card class="pa-8">
                <TheChoices/>
            </v-card>
        </v-row>
        <v-row>
            <v-card>
                <TheTitle/>
                <TheWord/>
                <TheButton/>
            </v-card>
        </v-row>
    </v-container>
</template>

<script>
import TheChoices from "./menu/TheChoices.vue"
import TheTitle from "./flashcard/TheTitle.vue"
import TheWord from "./flashcard/TheWord.vue"
import TheButton from "./flashcard/TheButton.vue"

export default {
    components: {
        TheChoices,
        TheTitle,
        TheWord,
        TheButton
    },
    data() {
        return {
            noChoice: true
        }
    }
}
</script>

<style>

</style>