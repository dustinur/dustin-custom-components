<template>
    <v-layout row>
        <v-flex xs12 sm6>
        <v-card>
            <v-toolbar color="grey">
            <!-- <v-toolbar-side-icon></v-toolbar-side-icon> -->

            <v-toolbar-title>Server Details</v-toolbar-title>
            <v-spacer></v-spacer>
            </v-toolbar>
            <v-list>
            <v-list-tile
                v-for="item in items"
                :key="item.id"
                avatar
                @click=""
            >
                <v-list-tile-action>
                <v-icon v-if="item.icon" color="pink">star</v-icon>
                </v-list-tile-action>

                <v-list-tile-content>
                    {{ item.server }} : {{ item.status }}
                </v-list-tile-content>

                <v-list-tile-avatar>
                <!-- <img :src="item.avatar"> -->
                <v-icon>info</v-icon>
                </v-list-tile-avatar>
            </v-list-tile>
            </v-list>
        </v-card>
        </v-flex>
    </v-layout>

</template>

<script>
export default {
    data () {
        return {
            items: [
                { server: 'Server 1', status: 'Live' },
                { server: 'Server 2', status: 'Live' },
                { server: 'Server 3', status: 'Live' },
                { server: 'Server 4', status: 'Live' },
                { server: 'Server 5', status: 'Down' }
            ]
        }
    }
}
</script>

<style scoped>
    .v-toolbar { color: white; padding: 0px;}
    ul {list-style: none;}
</style>
